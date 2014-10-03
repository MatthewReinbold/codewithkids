# Resetting the Google Coder Password

When setting up the Google Coder project on your Raspberry Pi (as defined elsewhere in this directory) you are required to enter a password before being able to complete any of the exercises. As is often the case, especially with kids, this password can be lost or forgotten. To reset the Google Coder password:

1. Navigate to the "**coder/coder-base**" directory in a terminal window.
2. Make a copy of the current configuration, located in "**device.json**". While it is *not* necessary, having a backup is a good habit to get into in the case that something goes wrong.
	1. Copy the contents of "**device.json**" to "**device.json.bkup**" by typing "**cp device.json device.json.bkup**".
	2. Check to make sure the new file exists by typing "**ls**".
3. With the original configuration saved, copy the contents of "**device.json.reset**" to "**device.json**". You do this by typing "**cp device.json.reset device.json**".

Start the node server running Google Code (or restart if it was already running). Now when you try and access Google Coder from the localhost browser it will ask you to create a password. Any previous application or modifications to projects *should still be there and unaffected*. 