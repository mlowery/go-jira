mkdir -p ~/src/go-jira/src/gopkg.in/Netflix-Skunkworks/go-jira.v0
cd ~/src/go-jira/src/gopkg.in/Netflix-Skunkworks/go-jira.v0
git clone https://github.com/Netflix-Skunkworks/go-jira.git .
GOPATH=~/src/go-jira go get -v gopkg.in/Netflix-Skunkworks/go-jira.v0 gopkg.in/Netflix-Skunkworks/go-jira.v0/main
GOPATH=~/src/go-jira go build -i -o ~/tmp/jira main/main.go
~/tmp/jira login
