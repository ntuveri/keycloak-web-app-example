# keycloak-web-app-example
Simple web app demonstrating basic usage of the Keycloak javascript client library
In this example the web app is supposed to run on localhost:8080, while Keycloak server is supposed to run on localhost:8090.
Keycloak versions 5 and 8 can be downloaded at: 
    * [Keycloak server v8](https://www.keycloak.org/archive/downloads-8.0.1.html)
    * [Keycloak server v5](https://www.keycloak.org/archive/downloads-5.0.0.html)

To run Keycloak server on port 8090 this command can be used: `C:\keycloak-8.0.1\bin>standalone.bat -Djboss.socket.binding.port-offset=10`

This repository contains:
     
    * [example-realm-v5.json](./example-realm-v5.json): the exported configuration of the client web app. The configuration have to be imported in Keycloak server version 5 
    * [example-realm-v8.json](./example-realm-v8.json): the exported configuration of the client web app. The configuration have to be imported in Keycloak server version 8
    * [webapp](./webapp/): the folder containing the web app resources 
    ..* [keycloak.json](./webapp/keycloak.json): the configuration of the web app related to Keycloak server
    ..* [index.html](./webapp/index.html): the main page of the web app demonstrating the library features (login, logout, show tokens, refresh token ...)
    ..* [silent-check-sso.html](./webapp/silent-check-sso.html): a callback page of the web app only needed to implement silent SSO


Below is the relevant documentation:
    * [Docs ](https://www.keycloak.org/docs/latest/securing_apps/#javascript-adapter-reference)
    * Original version of the [example web app](https://github.com/keycloak/keycloak/tree/master/examples/js-console)



