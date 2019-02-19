<h1>Setup-Developer-Linux</h1>

<h2>1) Install the VSCode</h2>

curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg

sudo install -o root -g root -m 644 microsoft.gpg /etc/apt/trusted.gpg.d/

sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main" > /etc/apt/sources.list.d/vscode.list'

sudo apt-get install apt-transport-http

sudo apt-get update

sudo apt-get install code


<h2>2) Configuring Code<h/2>

<h3>Install Dracula Official Theme</h3>

Install the extension Dracula

Click in File, Preferences, Color Theme

Digit Dracula and press Enter


<h3>Edit the Open Settings (JSON)</h3>

Press ctrl+shift+p

Digit Settings 

Select Preferences: Open Settings (JSON)

Add these configurations:

"editor.lineHeight": 24,

"editor.rulers": [80, 120],
  
"editor.tabSize": 2,
  
"editor.renderLineHighlight": "gutter",
  
"terminal.integrated.fontSize": 14,
  
"emmet.syntaxProfiles": {
  "javascript": "jsx"
},
  
"emmet.includeLanguages": {
  "javascript": "javascriptreact"
},
  
"javascript.updateImportsOnFileMove.enabled": "never",
  
"breadcrumbs.enabled": true,
  
"editor.parameterHints.enabled": false  
}


<h3>Install the vscode-icons</h3>

Install the extension vscode-icons
