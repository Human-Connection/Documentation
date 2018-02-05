# Docker

We are automatically builder Docker Images from the API and WebApp master branches with Travis CI where we also run tests.

#### ToDo's

* [ ] finish the doceker env documentation for the API
* [ ] finish the doceker env documentation for the WebApp

### API

#### Env Variables

| Env Var | Required | Default \(local\) | Description |
| :--- | :--- | :--- | :--- |
| HOST | ✓ | localhost | Host on which the api is running. |
| PORT | ✓ | 3030 | Port on which the api is running. |
| BASE\_URL | ✓ | [http://localhost:3030](http://localhost:3030) | Full API URL used for generating the upload urls. |
| FRONT\_URL | ✓ | [http://localhost:3000](http://localhost:3000) | Full WebApp URL used for in emails. |
| MONGO\_DB | ✓ | mongodb://localhost:27017/hc\_api | Connection URI used to connect to the Mongo Database. The credentials have to be included here on production. |
| SMTP\_HOST | ✓ | localhost | SMTP Host used for sending emails from locale or an 3th party service. |
| SMTP\_USER | ✓ | - | The SMTP User |
| THUMBOR\_URL | - | - | Optional URL to the Thumbor Service which generates Thumbnails on the fly, chaches and serves them.  |
| THUMBOR\_KEY | - \(recommanded for prod\) | - | The Thumbor Secret to prevent URL tempering. |
| AUTH\_SECRET | ✓ | - | A Secret which is used to salt sensitive date like the passwords etc. |
| EMAIL\_ADDRESS | ✓ | no-replay@human-connection.org | Email address used in outgoing emails. |

### WebApp

#### Env Variables



