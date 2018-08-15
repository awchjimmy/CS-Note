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
