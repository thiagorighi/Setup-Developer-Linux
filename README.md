<h1>Setup-Developer-Linux</h1>

<h2>1) Install the VSCode</h2>

curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg

sudo install -o root -g root -m 644 microsoft.gpg /etc/apt/trusted.gpg.d/

sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main" > /etc/apt/sources.list.d/vscode.list'

sudo apt-get install apt-transport-http

sudo apt-get update

sudo apt-get install code


<h2>2) Configuring Code<h/2>
