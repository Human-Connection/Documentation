# Docker

We are building Docker Images automatically from the API and WebApp master branches with Travis CI where we also run tests.

#### ToDo's

* [x] finish the docker env documentation for the API
* [x] finish the doceker env documentation for the WebApp
* [ ] Update Docker Compose Files

### API

#### ENV Variables

| ENV Var | Required | Default \(local\) | Description |
| :--- | :---: | :--- | :--- |
| HOST | ✓ | localhost | Host on which the api is running. |
| PORT | ✓ | 3030 | Port on which the API Server is running. |
| BASE\_URL | ✓ | [http://localhost:3030](http://localhost:3030) | Full API URL used for generating the Upload URL's. |
| FRONT\_URL | ✓ | [http://localhost:3000](http://localhost:3000) | Full WebApp URL used in Emails. |
| API\_SECRET | - | - | Used for the maintenance api toggle |
| MONGO\_DB | ✓ | mongodb://localhost:27017/hc\_api | Connection URI used to connect to the Mongo Database. The credentials have to be included here on production. |
| SMTP\_HOST | ✓ | localhost | SMTP Host used for sending emails from locale or an 3th party service. |
| SMTP\_USER | ✓ | - | The SMTP User |
| THUMBOR\_URL | - | - | Optional URL to the Thumbor Service which generates Thumbnails on the fly, chaches and serves them. |
| THUMBOR\_KEY | _recommended for prod_ | - | The Thumbor Secret to prevent URL tempering. |
| AUTH\_SECRET | ✓ | - | A Secret which is used to salt sensitive date like the passwords etc. |
| EMAIL\_ADDRESS | ✓ | no-replay@human-connection.org | Email address used in outgoing emails. |

### WebApp

#### ENV Variables

| ENV Var | Required | Default \(locale\) | Description |
| :--- | :---: | :--- | :--- |
| BASE\_URL | ✓ | [http://localhost](http://localhost) | Full URL used for generating URL's |
| HOST | ✓ | localhost | WebApp Server Host |
| PORT | ✓ | 3000 | WebApp Server Port |
| API\_HOST | ✓ | localhost | API Server Host |
| API\_PORT | ✓ | 3030 | API Server Port |
| SENTRY\_DNS\_PUBLIC |  |  | Logging Identifier used for debugging frontend and backend issues |
| MAPBOX\_TOKEN |  |  | Mapbox access token |
| RELEASE |  |  | Release Key which is replaced on build time to identify which issue affects which release |



