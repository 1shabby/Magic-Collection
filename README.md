Steps to connect GitHub Repo to ServiceNow:
1. Create / utilize the "PDI" fork
2. Import the application into your PDI from your fork of the ServiceNow repository
3. Create a branch from the tag for the module to begin with a partially built application
4. Authenticate GitHub in ServiceNow
     - Create a personal access token: https://github.com/settings/tokens
     - Store the token in a secure location
     - Create a credentials record on your PDI that utilizes the token
