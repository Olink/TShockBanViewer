TShockBanViewer
===============

Views all bans in your TShock database.

Install node.js.

execute: >npm install
execute: >node Server.js [portnum]

portnum is optional and defaults to 8000.

Ensure that your config.json has a token in it and ensure that it is correct.  The sample provided with the repo will
match your tshock.config.json file as well, see below.

TShocks Config:
To make this work, you need to tell TShock about your rest token you wish to use.
"ApplicationRestTokens": {
    "thisisasecureresttoken": {
      "Username": "BanViewer",
      "UserGroupName": "superadmin"
    }
  },
  
This is what mine looks like.  I have assigned the token "thisisasecureresttoken" to a user with the name BanViewer and
the permission level of superadmin.  You will notice that "thisisasecureresttoken" is what is in the node config file.
These must match and your server must be restarted in order for this application to work.  A basic display of errors and
bans has been added in the template folder.  Any modifications you wish to make can go there.  The public folder is for
things such as css or javascript you wish to link to.
