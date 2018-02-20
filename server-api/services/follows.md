# Follows Service

This Service has not an own database or table but manages entries inside the following service \(currently only users\) and the followed service \(users, organizations, projects\)

**GET /follows/$id**

List all services that the service with the given id follows

**POST /follows**

The user with the userId follows the service with the followingId specified by the type.

```
{
  "userId": "5a042f57a40ed49f79a328fb",
  "followingId": "5a042f5ca40ed49f79a32900",
  "type": "users"
}
```

## Todos {#todos}

* \[ \] Finish tests



