


Steps to install Go and setup for our Test Server - Kalpana, for MacOS : 

1. 	Open terminal
2. 	Execute the command -> brew install go
3. 	Check if the installation was successful with command -> go
4. 	Create a new Go workspace folder where you want and copy the path that command 'pwd' displays
5. 	Set GOPATH path using the response from above -> export GOPATH=*your local Go workspace location*
            eg. export GOPATH=/Users/a***/***/***/Go/go_workspace
6.      Creating subfolders in Go workspace from terminal -> mkdir -p $GOPATH $GOPATH/src $GOPATH/pkg $GOPATH/bin
7.	Go to Go workspace and check if you have src, bin and pkg folders we just created
8.	cd go_workspace/src
9.	git clone https://github.com/WWGSouthBay/kalpana.git -Cloning the git repository in our local workspace folder
10.	cd kalpana/
11.	make build - you should be able to see go get and go install being performed for our new project - kalpana
12. 	make serve - you should be able to see our test server has started and it displays the port it uses.
13. 	You have successfully started the server

Client Side testing of server : 

1. 	Once the server has started successfully using above steps, now lets test the server from Client end
2.	Keep the server running in its own terminal
3.	Open a new terminal and use the following command to test the connectivity between client-server
4.	curl http://localhost:3333   - This should give you term 'root.' in response. 
	Note : The port(3333) here might be different for your local system. Pick the one that server displays
5. 	curl http://localhost:3333/ping  - This should give you term 'pong' in response
6. 	Connectivity between client-server has been established successfully
