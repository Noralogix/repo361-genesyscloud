## Repo361 Genesys Cloud Raw Data 
1. Login to [Repo361](https://apps.repo361.com/) with AD credentials.
2. Go to settings page and generate client secret. Store it in a safe place. Next time secret will be hidden. 
3. Run Raw Data files API based on client credentials.

> **Note:** Repo361 is not storing api client secrets. For security purposes it just gives possibilities to create, update or delete secrets.  

Make post request with client credentials to generate auth token 
https://api.repo361.com/security/oauth2/token

Make get request with specified header Authorization
https://api.repo361.com/rawdata/files/{date}/csv

Where ***{date}*** in format yyyymmdd, for example 20210613

You can try [PowerShell](https://github.com/Noralogix/repo361-genesyscloud/blob/main/Repo361-RawData-API.ps1 ) example with your own clint credentials
