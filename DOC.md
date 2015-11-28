# DOCUMENTATION


## Preparation

### Scafold Initial App
The app's intial structure is scaffolded (yeoman) using StongLoop's Loopback API 
framework (The StrongLoop Framework must be installed - preferably Globally: npm install -g strongloop):

$ slc loopback

### Add Node & Express Intellisense support in VS Code
The primary development tool for this app is Visual Studio Code.  The editor's TypeScript support can be leveraged
to provide Intellisense support when editing Javascript files that reference the Node and Express 
libraries (The TypeScript Definition Manager must be installed - preferably Globally: npm install -g tsd):

$ tsd query node express --action install

after the install completes, a /typings folder is added to the project root.


