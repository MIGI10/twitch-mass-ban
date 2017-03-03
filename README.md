# Mass Ban application for Twitch Chat
This application is for banning a list of users in a text file from a twitch chatroom in a timely fashion.

# Disclaimer
## Needs Moderator Status in Chat!
This app must have moderator status in the chatroom that it will be doing the banning in. Be sure to connect it to an account that is trusted enough by the broadcaster to have moderator status or already has moderator status.

## Unauthorized usage!
Before using this app in someones twitch chat, please make sure that they are aware of the usage of it, that they know what it does, and that they have looked into it themselves to make sure it isnt malicious. Any issues that arise and have to do with unauthorized usage will be removed from the issue tracker! I will not tolerate improper usage then having someone come to me with a situation that was caused by improper usage! Please deal with that on your own accord!

# Installation
## Prerequisites
- **NodeJS v6.x.x LTS** - Can be downloaded from the [NodeJS Website](https://nodejs.org/en/)

## Instructions
### Global Instructions
- Download the latest release.
- Unzip the .zip file into its own folder.
- Open the folder that has all the file `index.js`.
- Please see the NPM Installation section for the OS you are using.
- Please see the .env file creation section.
- Installation is done.

### NPM Installation
- Open a terminal of somekind whether it be Bash, Windows Command Prompt or something else and navigate to the folder where the app was extracted to.
- Paste in the following command. `npm install`
- NodeJS will now get the required modules to run the app.
- Return back to the Global instructions.

### .env File Creation
- Create a file with the name of `.env` in the same folder as `index.js`. This will be used to store your Twitch Credentials.
- Open the file with your favoured text editor and copy/paste the following template.

- TwitchApps OAuth Token Generator: [TwitchApps](https://twitchapps.com/tmi/) << **Must be logged in with the account you want the app to run on!**

```
TWITCH_OAUTH=
TWITCH_USERNAME=
```

- Copy/paste the OAuth token you generated at the TwitchApps site after the `TWITCH_OAUTH=`
- Enter the username that you used for the token generation after `TWITCH_USERNAME=` *This will be the account that you are currently logged into the twitch website with*
- Return back to the Global instructions.

# Usage
*Remove any quotes when replacing values in the below command*  
`node index.js "username of chatroom to do banning in" "text file to pull names from (Each name must be on its own line)"`
