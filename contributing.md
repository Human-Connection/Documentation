# Contributing

## Contents

* [Introduction](contributing.md#Introduction)
* [Components Overview](contributing.md#Components-Overview)
* [Setup Development Environment](contributing.md#Setup-Developmen-Environment)

## Introduction

You want to contribute to the Human-Connection project? Great! Just read on!  
 Or are you still unsure how you could actually help? We've got you covered:  
 Head over to Opensource.Guide - there's an article that tells a lot about the Why and [How to contribute to Open Source](https://opensource.guide/how-to-contribute/) .  
   


## Components Overview

Human-Connection is build on its two main components: the server API and the Web-App.  
 Both are developed in separate repositories and can be run either locally or off a Docker image.  
 The HC documentation is in its own repository as well.  
   


## Get the code

### Clone the repositories

To explore and make changes to the files in the repository, you may want to clone it to your local disk.  
   
 You'll find them here on GitHub:  


> [Server API](https://github.com/Human-Connection/API)  
>  [Web App](https://github.com/Human-Connection/WebApp)  
>  [Documentation](https://github.com/Human-Connection/Documentation)  
>    
>
>
> ## Change the code
>
> If you see a problem, that you want to fix or know how to fix, feel free to create an issue in the corresponding repository. Issues that effect more than repository, should be created in the repository [Human-Connection](https://github.com/Human-Connection/Human-Connection) .  
>    
>
>
> ### Fork the code
>
> To change and commit the code, you will need to fork the repository, that you want to change files in, into your own GitHub.  
>  You need to have a login to [GitHub](https://github.com), and you can register for free, if you haven't already.  
>    
>  After that, you are able to clone this forked repository to your local system and begin to make changes in it.  
>  Add, fix, change the code as you wish. To make it easier for everyone maintaining or reviewing your code, you are encouraged to consider the [Coding Styleguide](web-app/installation.md#styleguide).  
>    
>  You can commit your changes to a new or to the same branch in your GitHub fork stating the issue number in the title, so it can easy be linked to by the repository owners, when it is ready to be merged.  
>    
>
>
> ## Test the code
>
> Unless you improve the documentation, you will want to test your changes . To do that, you need to setup the API and the Web App environments.   
>
>
> ### Setup Developer Environment
>
> There is a Docker and a local setup available for both parts - you are free to choose whatever you like:  
>    
>  [Setup the API via Docker](https://docs.human-connection.org/server-api/installation.html#setup-the-api-via-docker)  
>  [Setup the API locally](https://docs.human-connection.org/server-api/installation.html#setup-the-api-locally)  
>  [Setup the Web App via Docker](https://docs.human-connection.org/web-app/installation.html#setup-the-web-app-via-docker)  
>  [Setup the Web App locally](https://docs.human-connection.org/web-app/installation.html#setup-the-web-app-locally)  
>    
>
>
> ### Write test cases
>
> We are running tests with Travis CI.  
>    
>
>
> ### Ready to merge
>
> If your test cases work out, you can create a pull request, committing the changes you made to the HC repositories. The owners of this repository will then review the code and finally merge your contribution into the HC source.

