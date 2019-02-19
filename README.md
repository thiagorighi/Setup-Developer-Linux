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


<h3>Install Extensions</h3>

vscode-icons

Color Highlight

EditorConfig for VS Code

ESLint

Prettier - Code formatter

Rocketseat ReactJS

Rocketseat React Native


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

"prettier.eslintIntegration": true


<h2>3) Adding Google Chrome Extensions</h2>

<h3> Install these Extensions</h3>

react developer tools

dracula devtools theme

<h3> Configuring Dracula devtools theme</h3>

Paste in Google Chrome:
chrome://flags/#enable-devtools-experiments

Enable Developer Tools experiments

Relaunch

Press F12, Click Elements

Click three points menu (...), Settings 

Select Experiments and Allow custom UI themes

Enter in Rocketseat site
www.rocketseat.com.br

Inspect

Select React Menu (Elements, Console, .... React)

Click on the button Customize React DevTools

Choose the theme Dracula


<h2>4) Install Insomnia</h2>

echo "deb https://dl.bintray.com/getinsomnia/Insomnia /" \ | sudo tee -a /etc/apt/sources.list.d/insomnia.list
    
wget --quiet -O - https://insomnia.rest/keys/debian-public.key.asc \ | sudo apt-key add -

sudo apt-get update

sudo apt-get install insomnia

