### Upgrade 
- Node.js by reinstalling windows installer
- npm by 
	- running Powershell as Admin
	-  	Set-ExecutionPolicy Unrestricted -Scope CurrentUser -Force
	-  	npm install --global --production npm-windows-upgrade
	-  	npm-windows-upgrade

### Initialize New Project
- cd into new project directory
-     npm init
- yes to all
-     npm install package.json

You should have package.json, package-lock.json, and node_modules directory in the project directory

-    npm install react
-    npm install webpack webpack-cli --save-dev

--save-dev means you want to save the package to the webpack config
-    npm install svg-inline-loader --save-dev
-    npm install css-loader --save-dev
-    npm install style-loader --save-dev

to transform all js files into a format that is read by the browser, need to install babel
-    npm install babel-loader --save-dev

HTML webpack plugin will automatically create an html file that knows and includes the webpack bundle for us
-    npm install html-webpack-plugin --save-dev

