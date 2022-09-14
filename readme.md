### Docker Php App using Okta Demo

Goal: make a basic Php app that's able to use the Okta service for authentication (authN).

Okta article: https://developer.okta.com/blog/2018/07/09/five-minute-php-app-auth

Steps: 
1. Go to https://developer.okta.com/ and sign in (create an account if needed)
2. Applications > applications > Create app integration > choose OIDC > choose Web App > Next 
3. Name the app > set sign-in redirect URI: http://localhost:80/ (include the http and the trailing / char)
4. Do the same for the sign-out redirect URI: http://localhost:80/
5. Assignments > allow everyone in your org to access 
6. Copy the Client ID: 0oa6icqjxtDuNze4m5d7
7. Copy the Client Secret: OdW3QV3L_o2RrEgXqVd6EQLfvt9KJtOkPGkCvWeY
8. Make note of the Okta Org (in the URL of the Okta developer page: https://dev-96447452-admin.okta.com/)
9. Modify the values for the client id, secret, and okta org in the index.php file

To run code: 
1. Run cmd: `docker-compose up` from the project repo 
2. Go to: `http://localhost/:80` 

If you are getting errors, make sure that Docker is running on your local machine. 