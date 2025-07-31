Steps to connect GitHub Repo to ServiceNow:
On GitHub do the following:
1. Navigate to Settings > Developer Settings > Personal Access Tokens > Tokens (classic)
2. Navigate Generate new Token > Generate new Token (classic)
3. Change the name to something descriptive (I usually do 'PDI') and add all the Repo permissions. You can also set a token duration, I generally do No Expiration and let my PDI reset every so often.
4. Scroll to the bottom and create the token
5. You should be redirected to a new page where the token passphrase is present, be sure to copy it as you wont be able to do so again

On your ServiceNow Instance do the following:
1. In the filter navigator search for "credentials" and open the module sharing it's name
2. Create a new record
3. Select the type of "Basic Auth"
4. In the User Name field, enter your GitHub user name
5. In the Password field, paste the token passphrase we copied in step 5, part 1
6. Save the record
7. Navigate to Studio
8. In the header, click "Import App"
9. Make the following selections on the form:
     - Network Protocol : "HTTPS"
     - URL : put the URL link to the repo it should be in the form of "https://github.com/[UserName]/[RepoName].git"
     - Branch : set this to whatever branch you want to use, my repo has a "PDI" branch that I facilitate all things related to my PDI through so I set it to PDI (do note that this IS case sensitive)
     - Credential : here you should see the credential record we created listed  




Backlog:

1. Update widget to grab the src of the img tag instead of the value in the image field : Complete
4. Create a workspace to facilitate a back end agent experience
5. Integrate with PSDS / CSM to off a mock sales service
6. Potentially make a playtester / leverage Archidekt's playtester
