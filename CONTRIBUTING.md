# Contribute to Human-Connection

### Contents
* [Introduction](#Introduction)
* [Components Overview](#Components-Overview)
* [Setup Development Environment](#Setup-Developmen-Environment)


### Introduction
You want to contribute to the Human-Connection project? Great! Just read
on!<br />
You're still undecided how you could actually help? We've got you
covered:<br />
<br />
Head over to Opensource.Guide - there's an article that tells a lot
about the Why and
[How to contribute to Open Source](https://opensource.guide/how-to-contribute/)
.<br />
<br />
### Components Overview
Human-Connection is build on its two main components: the server API and
the Web-App.<br />
Both are developed in separate repositories and can be run either
locally or off a Docker image.<br />
Also the documentation is in its own repository.<br />
<br />
### Get the code
#### Clone the repositories
To explore and make changes to the files in the repository, you may want
to clone it to your local disk.<br />
<br />
You'll find them here on GitHub:<br />
[Server API](https://github.com/Human-Connection/API)<br />
[Web App](https://github.com/Human-Connection/WebApp)<br />
[Documentation](https://github.com/Human-Connection/Documentation)<br />
<br />
### Change the code
If you see an issue, that you want to fix or know how to fix, feel free
to open an issue in the corresponding repository. Issues that effect
more than repository, should be created in the repository
[Human-Connection](https://github.com/Human-Connection/Human-Connection)
.<br />
<br />
#### Fork the code
To change and commit the code, you will fork the repository, that you
want to change files in, into your own GitHub.<br />
You need to have a login to [GitHub](https://github.com), and you can
register for free, if you haven't already.<br />
<br />
After that, you are able to clone this forked repository to your local
system and begin to make changes in it.<br />
Add, fix, change the code as you wish. To make it easier for everyone
maintaining or reviewing your code, you are encouraged to consider the
[Coding Styleguide](web-app/installation.md#styleguide).<br />
<br />
You can commit your changes by creating a new branch in your GitHub fork
stating the issue number in the title, so it can easy be linked to by
the repository owners when it can be merged.<br />
<br />
### Test the code
To test your changes, you will need to setup the API and the Web App
environments.<br />
#### Setup Developer Environment
There is a Docker and a local setup available for both parts - you are
free to choose whatever you like:<br />
<br />
[Setup the API via Docker](https://docs.human-connection.org/server-api/installation.html#setup-the-api-via-docker)<br />
[Setup the API locally](https://docs.human-connection.org/server-api/installation.html#setup-the-api-locally)<br />
[Setup the Web App via Docker](https://docs.human-connection.org/web-app/installation.html#setup-the-web-app-via-docker)<br />
[Setup the Web App locally](https://docs.human-connection.org/web-app/installation.html#setup-the-web-app-locally)<br />
<br />
#### Write test cases
#### Ready to merge
If your test cases work out, you can create a pull request, committing
the changes you made to the HC repositories. The owners of this
repository will then review the code and finally merge your contribution
into the HC source.
