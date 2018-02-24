
# Kalpana

A Practice Web App project for the GO meetup group. 

#  Work List 
1. Build a Restful api
2. Build a UI using Go templates
3. Write tests
4. Add a Datastore
5. Dockersize
6. Deploy to Minikube


# Getting Started

Steps to install Go and setup for our Test Server - Kalpana, for MacOS : 

	1. 	Open terminal
	2. 	Execute the command -> brew install go
	3. 	Check if the installation was successful with command -> go
	4. 	Find home path for Go -> pwd
	5. 	Set GOHOME path using the response from above -> export GOPATH=*your local Go binary location*
	6. 	Create a new folder for Go workspace wherever you want
	7. 	Set GOPATH for Go workspace -> export GOPATH=$GOHOME/go_workspace 
        8. 	Set GOROOT for Go binary location  -> export GOROOT=/usr/local/opt/go/libexec
	9.	Set PATH with the above 2 GO PATHs -> export PATH=$PATH:$GOPATH/bin
						      export PATH=$PATH:$GOROOT/bin
	10.	Creating subfolders in Go workspace from terminal -> mkdir -p $GOPATH $GOPATH/src $GOPATH/pkg $GOPATH/bin
	11.	Go to Go workspace and check if you have src, bin and pkg folders we just created
	12.	cd go_workspace/src
	13.	git clone https://github.com/WWGSouthBay/kalpana.git - Cloning the git repository in our local workspace folder
	14.	cd kalpana/
	15.	make build - you should be able to see go get and go install being performed for our new project - kalpana
	16. 	make serve - you should be able to see our test server has started and it displays the port it uses.
	17. 	You have successfully started the server

Client Side testing of server : 
	1. 	Once the server has started successfully using above steps, now lets test the server from Client end
	2.	Keep the server running in its own terminal
	3.	Open a new terminal and use the following command to test the connectivity between client-server
	4.	curl http://localhost:3333   - This should give you term 'root.' in response. 
		Note : The port(3333) here might be different for your local system. Pick the one that server displays
	5. 	curl http://localhost:3333/ping  - This should give you term 'pong' in response
	6. 	Connectivity between client-server has been established successfully


