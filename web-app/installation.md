# Installation

## Setup the Web App via Docker

## Setup the Web App locally

### Installation

#### Build Setup

> we recommend to install the project locally for the best development ease and performance

```bash
# install dependencies
$ yarn

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn start
```

For detailed explanation on how things work, checkout the [Nuxt.js docs](https://github.com/nuxt/nuxt.js).

#### Env Vars

> More information on environment variables can be found in the [documentation (WIP)](https://docs.human-connection.org/environments/docker-test-production/docker-configuration.html)

#### Maintenance

You can start the app in maintenance mode so it does not ask the api in case it is down.
```
$ env MAINTENANCE=true yarn dev 
# or start
$ env MAINTENANCE=true yarn start
```

#### Test Logins

**Admin**

E-Mail: `test@test.de`  
Password: `1234`

**Moderator**

E-Mail: `test2@test2.de`  
Password: `1234`

**Normal User**

E-Mail: `test3@test3.de`  
Password: `1234`

#### Styleguide

> Note: The Styleguide is currently broken as we can't use the webpack config from nuxt.js at the moment. If you find a way to fix that issue, please feel free to open a pull-request

The Developer Style Guide provides important infos about components and styles. To start it simply type:

```bash
$ npm run styleguide
```

When built you can open it at [http://localhost:6060](http://localhost:6060)

#### Backpack

We use [backpack](https://github.com/palmerhq/backpack) to watch and build the application, so you can use the latest ES6 features \(module syntax, async/await, etc.\).
