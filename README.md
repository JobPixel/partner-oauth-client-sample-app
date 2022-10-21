 # partner-oauth-client-sample-app (boilerplate)
This repository contains a sample oauth client

The JobPixel partner API is OAuth 2 based.  In order to use this client application, you will need authorized API credentials issued to you by JobPixel.  Upon receipt, these credentials will need to be updated in the routes/index.js file

## Installation

This requires [Node.js](https://nodejs.org/) v12+ to run.

Install the dependencies and devDependencies and start the server.

```sh
git clone git@github.com:JobPixel/partner-oauth-client-sample-app.git
npm i
npm start
```

Note: Your app must be running on localhost:3000, if you don't have that port available you can change that in `./bin/www`

## ToDo

- update `clientId` and `clientSecret` in routes/index.js
- visit `/auth` to see the sample /authorize url -  this will redirect to JobPixel with the query string - here you have to use the provided credentials which will then redirect to callback url specified in the previous step
- use this authorization code to generate the access token and refresh token (authorization_code grant)
- in case access token expires, use token api to get the new token (refresh_token grant)

## License

MIT

**Free Software, Hell Yeah!**
