# Docker Installation


_More information will follow shortly_

# Local Installation

Run:

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# build once and launch server
$ yarn build
$ yarn start
```

For detailed explanation on how things work, checkout the [Nuxt.js docs](https://github.com/nuxt/nuxt.js).

## Env Vars

> More information on environment variables can be found in the [documentation \(WIP\)](https://docs.human-connection.org/environments/docker-test-production/docker-configuration.html)

#### Test Logins

| Role | E-Mail | Password |
| :--- | :--- | :--- |
| Admin | test@test.de | 1234 |
| Moderator | test2@test2.de | 1234 |
| User | test3@test3.de | 1234 |

#### Styleguide

The Developer Style Guide provides important infos about components and styles. To start it simply type:

```bash
$ yarn run styleguide
```

When built you can open it at [http://localhost:6060](http://localhost:6060)

#### Backpack

We use [backpack](https://github.com/palmerhq/backpack) to watch and build the application, so you can use the latest ES6 features \(module syntax, async/await, etc.\).

