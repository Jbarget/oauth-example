# A barebones oAuth example with Github + request for Github data

We are using:
- Github oAuth to authenticate a user
- Hapi server to deal with requests

Steps to get it working:

1. Clone the repo
2. Move into the directory by typing `cd oauth-example` into your terminal
3. Go here and register a new application https://github.com/settings/developers
4. Enter an application name
5. Set the Homepage URL to : http://localhost:8000
6. Set the Authorization Callback URL to: http://localhost:8000/welcome. And click register application
7. create a config.env file in the root of the project directory and enter this info:

  `GITHUB_CLIENT_ID= *your application's client ID*`
  
  `GITHUB_CLIENT_SECRET= *your application's client secret*`
  
  `BASE_URL=http://localhost:8000`
  
8. run the server `node lib/server.js` and go to: http://localhost:8000/login

