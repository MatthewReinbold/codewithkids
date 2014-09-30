# Adjusting Screen Offsets

Sometimes after plugging in a Raspberry Pi to a new monitor the display will be "off". This is how to adjust the screen.

1. Log in after booting up (enter the username and password - "pi" and "raspberry" if still using defaults.
2. At the bash prompt (the "$" symbol prior to the blinking cursor), type "**sudo nano /boot/config.txt**"
3. In the screen that appears, type the following command for how things need to be moved. If the text is off the screen to the left, type "**overscan_left=100**" at the bottom of the file. 
4. Type "**ctrl** and the "**X**" key simultaneously to save the contents of the file.
5. Type "**Y**" to confirm that you'd like to save the file. 
6. Restart the Pi to have the changes take effect: "**sudo poweroff**"