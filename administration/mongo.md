# Setup mongo cluster

First of all, start your mongo docker container in rancher with `command` parameter `--port 27017` (or anything which is *not* `--auth`, see below).

Connect with your server via SSH and get the container id of the running mongo cluster:
```sh
sudo docker ps
```

Connect to the mongo client in the docker container
```
sudo docker exec -it <docker_id> mongo
```

Use the mongo client to setup authentication:
```sh
use admin;
# replace rootUserPassword with your own secure password
db.createUser({user:"su", pwd:"rootUserPassword",roles:["root"]});
db.auth("su", "rootUserPassword");

# add external users with minimal required permissions for their corresponding tables
use hc_api;
# replace apiUserPassword with your own secure password
db.createUser({user:"hc-api", pwd:"apiUserPassword",roles:["readWrite"]});

use embed_api;
# replace embedApiUserPassword with your own secure password
db.createUser({user:"hc-embed-api", pwd:"embedApiUserPassword",roles:["readWrite"]});

```

After creating one root user and the required external users we need to restart the mongo docker image with `command` parameter `--auth` to enforce authentication.
