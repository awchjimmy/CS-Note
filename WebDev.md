# Web Development Notes

- Enable Web Bluetooth (Linux)
```
1. Go to url: chrome://flags
2. Enable 'Experimental Web Platform features'
3. Restart Chrome
```

### Auth Background Knowledge
- OAuth 2.0, OpenID Connect and JWT – What are they and why do you care? - Pt1 -  
https://communities.ca.com/community/ca-security/ca-single-sign-on/blog/2016/04/29/oauth-openid-connect-and-jwt-what-are-they-and-why-do-you-care-part-1-of-2

- Token Authentication: The Secret to Scalable User Management -  
https://stormpath.com/blog/token-authentication-scalable-user-mgmt

- https://auth0.com/blog/the-difference-between-wam-and-idm/ -  
https://auth0.com/blog/the-difference-between-wam-and-idm/

- Introduction to JSON Web Tokens -  
https://jwt.io/introduction/

### Auth Implementation
- Authenticate your Firebase users with Instagram -  
https://firebase.googleblog.com/2016/10/authenticate-your-firebase-users-with.html

- OAuth2 Python Example -  
https://github.com/reddit-archive/reddit/wiki/OAuth2-Python-Example

- 跟我学Shiro -  
http://jinnianshilongnian.iteye.com/blog/2018398

- Control Access with Custom Claims and Security Rules -  
https://firebase.google.com/docs/auth/admin/custom-claims

### JS Related
- A guide to writing asynchronous JavaScript programs -  
http://callbackhell.com/

### Handy Tools
- ngrok - secure introspectable tunnels to localhost -  
https://ngrok.com/download

- localtunnel - expose yourself -  
```
$ sudo npm install localtunnel -g
```

- jsDelivr - A free, fast, and reliable Open Source CDN for npm & GitHub -  
https://www.jsdelivr.com/

### VS Code

| key | description |
| ---- | ---- |
| ```M + /``` | toggle comment |
| ```:%s/oldText/newText/g``` | global replace (vim) |

### CLI Quick Tips
| Command / Partial Command | description | example |
| ---- | ---- | ---- |
| !! | previous input command | sudo !! |
| - | standard input | cat hello.txt \| diff world.txt - |
