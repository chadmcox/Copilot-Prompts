# Copilot-Prompts
## Prompts that work
* user with accountname ***change_me*** is receiving multiple bad passwords while trying to logon to Active Directory what computer are they trying to logon from. this information should be found in Defender.
* when was the last time accountname ***change_me*** password was changed this data should be found in defender (note this will only show last 30 days).
* what application is upn ***change_me*** logging onto over last 7 days. this information shuld be found in defender
* can you retrieve a list of sensitve accounts that are in the identity info table from defender
* over the last 7 days ***change_me*** was being prompted to MFA. which conditional access policy was causing that. this information should be in defender the table to use is AADSignInEventsBeta
* over the last 7 days ***change_me*** was logged in from multiple locations. provide that list in a table. this information should be in defender the table to use is AADSignInEventsBeta
* follow up:  /askGPT can you summarize the locations and is there anything unusual about them
* /askGPT what is the application: Microsoft Azure Active Directory Connect used for in Azure AD
* follow up: are there any threat indicators that involve that application
* retrieve a list of users, errorcodes, country, state, city and ipaddress that have tried to sign-in to application id 'cb1056e2-e479-49de-ae31-7812af012ed8' in entra over the last 7 days. This data should be found in defender in the AADSignInEventsBeta table
* has upn ***change_me*** signed in over the last 7 days from a device that is not compliant 

## Prompts I want to test or build
* What is x signing into on premise
* What is x signing into in Azure
* What devices is x using
* What changes has x made in Entra
* Does x have any known user risk
* Show applications x has failed to sign into
* Has x account been locked out and why
* Does x have any sign-ins from unknown devices
* Give me locations x has signed in from.
* Give me a list of accounts that might be involved with a password spray
* Does x have any known roles or is flagged as sensitive
* Has any taps been issued to global admins
* Has the entra connect syncronization account accessed anything other than the azure ad connect application
* Has the entra connect syncronization account done anything unusual
* Has the entra connect syncronization account been issued a tap
* What changes has global admin accounts made recently
* Any bad password attempts against global admin accounts
* Have any cloud only accounts been created
* List conditional access policies recently updated or added
* What changes have been made to entra roles lately
* what changes have been made to domains admins
* what changes have been made to enterprise admins
* what changes have been made to schema admins
* give recent added permissions to applications in entra
* why is user not able to change password
* any users with deny or report as suspicious mfa responses
* what mfa methods is the user using
* has x recently registered an mfa method
* what applications are guest signing into
* who consented to a permission
* what users have been issued a temporary access pass
* what users recently change mfa with a risk


This is resources for various prompts I find useful.

* [User Sign in Analysis](https://github.com/Azure/Copilot-For-Security/blob/main/Promptbook%20samples/User%20Sign%20in%20Analysis%20and%20Investigation%20Promptbook.md)
* [Copilot for Security sample prompt collection](https://github.com/Azure/Copilot-For-Security/tree/main/Sample%20Prompts)
