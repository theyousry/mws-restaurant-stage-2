# Mobile Web Specialist Certification Course
---
#### _Three Stage Course Material Project - Restaurant Reviews_

## Project Overview: Stage 2

For the **Restaurant Reviews** projects, you will incrementally convert a static webpage to a mobile-ready web application. In **Stage Two**, you will take the responsive, accessible design you built in Stage One and connect it to an external server. You’ll begin by using asynchronous JavaScript to request JSON data from the server. You’ll store data received from the server in an offline database using IndexedDB, which will create an app shell architecture. Finally, you’ll work to optimize your site to meet performance benchmarks, which you’ll test using **Lighthouse**.

## Specification

You will be provided code for a Node development server and a **README** for getting the server up and running locally on your computer. The **README** will also contain the **API** you will need to make **JSON** requests to the server. Once you have the server up, you will begin the work of improving your Stage One project code.

The core functionality of the application will not change for this stage. Only the source of the data will change. You will use the **fetch() API** to make requests to the server to populate the content of your **Restaurant Reviews** app.


## Requirements

Use server data instead of local memory In the first version of the application, all of the data for the restaurants was stored in the local application. You will need to change this behavior so that you are pulling all of your data from the server instead, and using the response data to generate the restaurant information on the main page and the detail page.

Use **IndexedDB** to cache **JSON** responses In order to maintain offline use with the development server you will need to update the service worker to store the **JSON** received by your requests using the IndexedDB API. As with Stage One, any page that has been visited by the user should be available offline, with data pulled from the shell database.

Meet the minimum performance requirements Once you have your app working with the server and working in offline mode, you’ll need to measure your site performance using Lighthouse.

### Lighthouse measures performance in four areas, but your review will focus on three:

* Progressive Web App score should be at 90 or better.
* Performance score should be at 70 or better.
* Accessibility score should be at 90 or better.

You can audit your site's performance with Lighthouse by using the Audit tab of Chrome Dev Tools.

## Getting Started

### Run the App
##### Navigate into Front-End directory
```
# cd App _ Front-End
```
##### In a terminal, check the version of Python you have:
```
# python -V
```
#####If you have Python 2.x spin up the server with
```
# python -m SimpleHTTPServer 8000
```
`(or some other port, if port 8000 is already in use.)`
#####For Python 3.x, you can use
```
# python3 -m http.server 8000
```
#####If you don't have Python installed, navigate to Python's[website](https://www.python.org/)
`to download and install the software.`

#####With your server running, visit the site:
```
http://localhost:8000
```
### Development local API Server
_Location of server = /server_
Server depends on [node.js LTS Version: v6.11.2 ](https://nodejs.org/en/download/), [npm](https://www.npmjs.com/get-npm), and [sails.js](http://sailsjs.com/)
Please make sure you have these installed before proceeding forward.

Great, you are ready to proceed forward; awesome!

Let's start with running commands in your terminal, known as command line interface (CLI)

### Run the Server
##### Navigate into Back-End directory
```
# cd Server _ Back-End
```
###### Install project dependancies
```Install project dependancies
# npm i
```
###### Install Sails.js globally
```Install sails global
# npm i sails -g
```
###### Start the server
```Start server
# node server
```
### You should now have access to your API server environment
debug: Environment : development
debug: Port        : 1337
