# verificationbot
 A Polymart verification Discord bot made in Python \
 This bot is made specifically for Oraxen Discord server.

# How to use?
 First get Python 3, then use pip to install `requests interactions`.

# First time setup
 * Create a new bot in [Discord Developer Portal](https://discord.com/developers/applications) (make sure to sign in to your Discord account first), then go to Bot settings, generate a Bot token and copy that token. Open the verify.py file and replace the placeholder in the token variable with your Bot token you have copied.
 * Now come to OAuth2 settings and select "URL Generator". Here in the "Scope" section select "bot" and "application.commands" (bot is self explaintory, application.commands is for slash commands). After that in the Permission selection give the boot "Administrator" permission. Now it should generate a bot invite link for you. Copy that URL in the "Generated URL" box by clicking the Copy button and use that link to invite the bot into your Discord server.
 * Now you need a role that the bot give the user if verification process successful. You can tweak, edit that role whatever you want. After that copy the ID of that role by right clicking to the role in the Role settings screen and click the "Copy ID" button, paste it into the "verified_role_id" variable in the verify.py file.
 * If you want to restrict API key operation (adding/deleting API key) to yourself only (for security purposes, recommended), you may want to get your user ID by right clicking to your user profile and smash the "Copy ID" button (jokin') and paste it to the "owner" variable in the verify.py file, also make sure to set the "restrict_api_operation_to_owner" variable to "True" (capital T matters). Else if you don't want that, leave the "owner" variable empty and set the "restrict_api_operation_to_owner" variable to "False" (capital F matters also). If you do not restrict API operation to yourself it will default access to who have the "Administrator" permission.
 * Now you need to get your Discord Server's ID by right clicking to the server and click "Copy ID", then paste it to the "server_id" variable.
 * Now you are all set! Open your favorite terminal emulator (or Command Prompt) and run the verify.py file using Python 3 and enjoy!
