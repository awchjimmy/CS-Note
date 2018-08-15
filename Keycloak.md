### Environment Setup
- Ubuntu 16.04
- Keycloak 4.2.1.Final
- openjdk-8-jdk

### SSH Tunnel for Administrative tasks
- Create a tunnel
```
# $ ssh -L <locol-source-port>:<remote-dest-hostname>:<remote-dest-port> -i path/to/key server-user@server-hostname

# e.g.
$ ssh -L 8080:localhost:8080 -i path/to/key.pem ubuntu@example.com
```
keywords: ssh local port forwarding

### Create Admin Account
```
$ bin/add-user-keycloak.sh -r master -u <username> -p <password>
```
ref: https://www.keycloak.org/docs/4.2/server_admin/

---

### Creating a Realm and User
ref: https://www.keycloak.org/docs/latest/getting_started/index.html#creating-a-realm-and-user
