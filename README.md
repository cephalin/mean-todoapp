---
languages:
- nodejs
- javascript
page_type: sample
description: "This is a sample application that you can use to follow along with the Build a Node.js and MongoDB web app in Azure tutorial."
products:
- azure
- azure-app-service
---

# Todo App on the MEAN stack for Azure App Service

This is a [Sails.js](https://sailsjs.com) and Angular application you can use to follow along with the tutorial at [Build a Node.js and MongoDB web app in Azure](https://docs.microsoft.com/azure/app-service/tutorial-nodejs-mongodb-app).

### Overview

- The app is generated using the [Sails.js CLI](https://sailsjs.com/documentation/reference/command-line-interface) and serves an API called `Todo`. Other modifications:
    - Views and sockets are disabled (see `.sailsrc`).
    - In `config/production.js`, `sails.config.http.trustProxy` is set to `true`.
- The `client` directory contains an Angular 12 client app, generated using the [Angular CLI](https://angular.io/cli/new).
- To build the Angular client app anytime, run `npm run build` (see `package.json`). The command runs `ng build` and moves the output to the `assets` directory, which Sails.js uses to serve static files.
- To run the app in the development environment, run [`sails lift`](https://sailsjs.com/documentation/reference/command-line-interface/sails-lift) or `node app.js`.
- The `start` script in `package.json` is run by Azure App Service by default to start up the app.

### Links

+ [Sails framework documentation](https://sailsjs.com/get-started)

### Version info

This app was originally generated on Tue Jul 06 2021 14:54:05 GMT+0200 (Central European Summer Time) using Sails v1.4.3.

<!-- Internally, Sails used [`sails-generate@2.0.3`](https://github.com/balderdashy/sails-generate/tree/v2.0.3/lib/core-generators/new). -->

<!--
Note:  Generators are usually run using the globally-installed `sails` CLI (command-line interface).  This CLI version is _environment-specific_ rather than app-specific, thus over time, as a project's dependencies are upgraded or the project is worked on by different developers on different computers using different versions of Node.js, the Sails dependency in its package.json file may differ from the globally-installed Sails CLI release it was originally generated with.  (Be sure to always check out the relevant [upgrading guides](https://sailsjs.com/upgrading) before upgrading the version of Sails used by your app.  If you're stuck, [get help here](https://sailsjs.com/support).)
-->

## Contributing

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
