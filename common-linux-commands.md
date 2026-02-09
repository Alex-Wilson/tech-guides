# Hello, Tux!
This guide will be focused on use in Arch based linux enviornments, specifically CachyOS. This guide assumes succesful installation of CachyOS. 

I’d just like to interject for a moment. What you’re refering to as Linux, is in fact, GNU/Linux, or as I’ve recently taken to calling it, GNU plus Linux. Linux is not an operating system unto itself, but rather another free component of a fully functioning GNU system made useful by the GNU corelibs, shell utilities and vital system components comprising a full OS as defined by POSIX.

Many computer users run a modified version of the GNU system every day, without realizing it. Through a peculiar turn of events, the version of GNU which is widely used today is often called Linux, and many of its users are not aware that it is basically the GNU system, developed by the GNU Project.

There really is a Linux, and these people are using it, but it is just a part of the system they use. Linux is the kernel: the program in the system that allocates the machine’s resources to the other programs that you run. The kernel is an essential part of an operating system, but useless by itself; it can only function in the context of a complete operating system. Linux is normally used in combination with the GNU operating system: the whole system is basically GNU with Linux added, or GNU/Linux. All the so-called Linux distributions are really distributions of GNU/Linux!

# Resources and Refereces

[Arch Wiki](https://wiki.archlinux.org/title/Main_page)
Many have polarized views about Arch because of elitiest toxicity of the community. I am here to reassure you that Arch in fact does the opposite. They provide a path to mastery by having a comprehensive wiki and an active community. The same community that will flame windows will help strangers debug niche CAD software they themselves do not even use. Largely to teach themselves more and more.  This is because the community takes itself seriously (as far as understanding, maintaining, and developing arch). Someone has likely already experienced the same issues you face now, try to learn from them as much as possible.

[Cachy Wiki](https://wiki.cachyos.org/)
Cachy and other forks of Arch (CachyOS, Omarchy, EndeavourOS) are becomming increasinly popular for the same reason they are so hated among the "arch-cel" community. These distrubutions subvert the philosophies of Arch like configurability, maintainability, extensiblity, modularity, customizability, and pionneering by removing user choice. Something seen as holy to the arch community. 

Those who partook in the pilgramige of self discovery to create and innovate Arch, people who "enjoy" the "scenic serenity" of setting up deprecated Wi-Fi drivers from their terminal for no pay, cleared the path through the chaos. Those forerunners encouraged others to walk the same path for their destination was built only through their own toil. The knew people would learn more by failing to compile shaders for a video game than any 16-week university class could teach them. This is because those users felt the impact of what they were building and they were free to share that impact with the world, one commit at a time. 

As more and more people walked this path it expanded, people estblished the first metaphorical streets and roads. The strife of set up, the personilization of the user experience, and general capacity for expression in Linux became signifiers of an "arch user". Many best practices formed, expanded, and became standards which did homogenize the user base but the users still had a tool box to make their experience unique.

Slowly, then all at once. Everything changed when archinstall came out. It was a simple script that helped to automate the installation of Arch to relative perfection. To continue our path anology, this would be like an 8-lane highway next to an airport near a train station. People realized that there was a low barrier of entry to the OS market now that they could use arch as a starting point and then dress it up to their liking. This goal to be the personal use standard Linux distro has been achieved. 

Now there is fear that the team who earned the glory of Arch will be dethroned by a more exploitative competitor. Likely an adversary who attacks Arch directly, introduces proprietary technology, and can out develop/capitalize arch, ultimately replacting or consuming them. As we have seen in other technologies, the race to simplification is often rewarded with ubiquity. This is why "arch-cels" cringe when Cachy users select a window manager from a dropdown in a GUI durring setup. The choice is obfuscated by abstaction. The user might not even know they can choose other options or older versions or just not use one, just like how customers at McDonalds do not think of the conditions of the animals they consume or the logistics of how it got their despite the impact those things have on them. This goes against the "build and do it yourself" mentality which has always been a core belief of Linux developers.     

In my opinion Cachy is philsophically aligned with Arch as it helps to combine the great aspects of arch into a pre-congigured pacakge with GUI programs, desktop enviornments, window managers, compiler optimiazations, and thir own twists on the endless extensibility and customizability of Arch. Think of Cachy as an extention or a coat of pain on top of Arch. Its even possible to convert CachyOS back to Arch with enough patience. 

We will be using CachyOS for this guide. 


# Commmand Line Interface, Terminals, and Shells, Oh My! 

**Graphical User Interface (GUI):** A GUI is the most common way to interface with computers, electronic devices, and computer programs. Think of pressing the buttons to construct a text on your phone, using your mouse to click a color in a spreasheet, changing the settings in the menu of a video game, or pressing "resume printing" on a printer's screen that ran out of paper. In all these scenarios the user is interacting with the the computer through a GUI, allowing the user to make changes to the computer or program by clicking buttons, moving sliders, "dragging and dropping", and/or touching a screen. GUIs are easy to learn and also help to express what the computer or application to do.

**Command Line Interface (CLI):** A command line interface, an alternative to the GUI, is also a way to interact with a computer or program. Instead of manipulating graphical elements like toggles, sliders, and buttons, the command line almost exlusively uses commands sent from the keyboard. Consider muting the audio on a computer. In a GUI enviornment (like windows) you likely press the speaker button, then click "sound", then move the slider to the left/bottom or press the "mute" button. 

 Instead of a muting the audio with a button or knob the user might type "volume -100%". This is not an actual command but its simmilar to how the CLI is different. This might seem like an archaic and difficult way to interact with the computer but it is very explicit, well defined, and programmable. Most computers use this type of interface under the hood anyway.  

**Terminal:** The terminal is the hardware or software that provides a way to interact with the computer's input and out put. In the past terminals were dedicated devices, typically consisting of a keyboard (input device) and a built in monitor (output device) that would be plugged into a larger computer which would operate (normally) without a keyboard, mouse, or screen. The terminal was a "window" that allows the user to interact with the machine. This is what Neo is using in the Matrix, where the screen had a bunch of green text on screen. In modern times the terminal is a piece of software that serves the same function, rendering text on screen, capturing keystrokes, handling copy/pasting, scrolling, resizing, etc.

**Shell:** The shell is the unerlying program in the terminal or command line interface. Consider Alacritty, which is a terminal emulator. This program allows me to use different fonts, set keyboard shortcuts, and change the color of the windows and text on screen. I type into Alacritty if I want to make a file or rename a file but the underlying shell (Fish/Bash) is what actually creates or renames the file when I give the command. Bash is the main Linux shell. It has pre-programmed commands that the computer knows how to execute just by typing those commands and hitting enter. Creating a file is done with "touch" and renaming a file can be accomplished with "mv". Its important to note that there is often no visual feedback from the shell and we need to use them carefuly and investigate the impact of our commands. Typing "Make alex have straight A+s" is not a valid command so nothing will happen.    

**Terminal User Interface (TUI):** This is a modern paradigm which combines the direct action, programability, and features of a command line interface with the information, customization, and ease of use of a GUI. For example it is hard to edit large text files directly in the terminal from the command line but we can use tools that utilize a TUI, like Neovim to make it easier without leaving the terminal. This is like an "app" that runs in the terminal. Once we launch Neovim we are greeted with a complete change in what each button and command does with different capabilities than the normal terminal or even shell.  


The command line can be found by pressing the windows (called the modification key in the linux world) and the "enter" key. We cam denote keyboard combinations with the following notation "mod" + "enter" => terminal





## Processses, Threads, Users, and Process ID Numbers in Linux

## Files and Directories in Linux

Each program and process has a user associated with it. There are three main types of users. There is the root user (also known as the host) which  also known as the host in virtualized enviornments, and then there is the 

## Finding the currently logged in user with whoami
## Finding working directory with pwd

## List the contents of a directory with ls

ls 


## Creating a directory with mkdir
Creates a new directory

mkdir new-directory


## Creating a file with touch
Creates an empty file with a given name

touch new-file.txt

## Renaming a file with mv command

cd ..
mv old-folder-name new-folder-name
cd new-folder-name

## Removing a File or Directory with rm


## Navigation (pwd, cd, ls)
## File Operations (cp, mv, rm, mkdir, touch)
## Reading Files (cat, less, head, tail)
## System Information (neofetch, btop, df, free)
## Common Applications and Alternatives (nvim, codium, zen)

# Hyperland Commands

## Full sizing a window
## Minimizing a window
## Closing a window
## Switching windows
## Tiling a window
## Congifuring dot (.) files
