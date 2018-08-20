### 簡單統整

#### 完成
##### Keycloak
- 本地安裝 keycloak
- username / password 帳號管理
- role / group 角色群組 權限設定
##### Nodejs (Optional)
- username / password 登入登出
- role / group 權限應用

#### 未完成
- http -> https
- 第三方 google 整合
- 第三方 fb 整合
- 防護 Java app
---

### Environment Setup
- Ubuntu 16.04
- Keycloak 4.3.0.Final
- openjdk-8-jdk

### SSH Tunnel for Administrative tasks
- Create a tunnel
```
# $ ssh -L <locol-source-port>:<remote-dest-hostname>:<remote-dest-port> -i path/to/key server-user@server-hostname

# e.g.
$ ssh -L 8080:localhost:8080 -i path/to/key.pem ubuntu@example.com
```
keywords: ```ssh local port forwarding```

---

### Creating an Admin Account
```
$ bin/add-user-keycloak.sh -r master -u <username> -p <password>
```
ref: https://www.keycloak.org/docs/4.2/server_admin/

### Creating a Realm and User
ref: https://www.keycloak.org/docs/latest/getting_started/index.html#creating-a-realm-and-user

---

### Securing Node App
ref: https://www.keycloak.org/docs/latest/securing_apps/index.html#_nodejs_adapter  
ref: https://github.com/keycloak/keycloak-nodejs-connect/blob/master/example/index.js  
PS: It's a STATEFUL solution, so we must setup some kind of memory store. e.g. express-session. Currently, not sure how to change to a STATELESS one.

### Role-based Authorization
#### Role & Group Setup
ref: https://www.keycloak.org/docs/latest/server_admin/index.html#roles  
ref: https://www.keycloak.org/docs/latest/server_admin/index.html#groups  
#### App(Client) Role Syntax
```
app.get( '/extra-special', keycloak.protect('other-app:special'), extraSpecialHandler );
```
ref: https://www.keycloak.org/docs/latest/securing_apps/index.html#usage-2
