This guide will be focused on use in Arch based linux enviornments, specifically CachyOS. This guide assumes succesful installation of CachyOS. 

I’d just like to interject for a moment. What you’re refering to as Linux, is in fact, GNU/Linux, or as I’ve recently taken to calling it, GNU plus Linux. Linux is not an operating system unto itself, but rather another free component of a fully functioning GNU system made useful by the GNU corelibs, shell utilities and vital system components comprising a full OS as defined by POSIX.

Many computer users run a modified version of the GNU system every day, without realizing it. Through a peculiar turn of events, the version of GNU which is widely used today is often called Linux, and many of its users are not aware that it is basically the GNU system, developed by the GNU Project.

There really is a Linux, and these people are using it, but it is just a part of the system they use. Linux is the kernel: the program in the system that allocates the machine’s resources to the other programs that you run. The kernel is an essential part of an operating system, but useless by itself; it can only function in the context of a complete operating system. Linux is normally used in combination with the GNU operating system: the whole system is basically GNU with Linux added, or GNU/Linux. All the so-called Linux distributions are really distributions of GNU/Linux!



# Resources and Refereces

Arch Wiki(https://wiki.archlinux.org/title/Main_page)
Many have polarized views about Arch because of elitiest toxicity of the community. I am here to reassure you that Arch in fact does the opposite. They provide a path to mastery by having a comprehensive wiki and active community. The same community that will flame windows will help people debug niche CAD software they dont even use themselves.  This is because the community takes itself seriously (as far as understanding, maintaining, and developing arch). Someone has likely already experienced the same issues you face now, try to learn from them as much as possible.

Cachy Wiki(https://wiki.cachyos.org/)
Cachy and other forks of Arch (CachyOS, Omarchy, EndeavourOS) are becomming increasinly popular for the same reason they are so hated among the "arch-cel" community. These distrubutions take the philosophies  of Arch like configurability, maintainability, extensiblity, modularity, customizability, and pionneering and subvert them. 

Those who partook in the pilgraimage of self discovery to create and innovate Arch, people who "enjoy" the "scenic serenity" of setting up Wi-Fi drivers from their terminal for no pay, cleared the path through the chaos. Those forerunners encouraged others to walk the same path for their destination was built only through their own toil. People will learn more by failing to compile shaders for a video game they want to play than anyone could teach them in a 16-week class. People were building something for themselves, their friends, and humanity, not just a grade. They felt the impact of others and shared thier own contributions one commit at a time. As more and more people walked this path it expanded, people estblished the first metaporical streets and roads. The strife of set up, the personilization of the user experience, and general capacity for expression in Linux became signifiers of an "arch user". Many best practices formed, expanded, and became standards. Users could start to feel themselves merge into one another. They were becoming homogenized despite their best efforts to stay customizable and despsite insane capactiy for uniqness.  

Slowly, then all at once. Everything changed when archinstall came out. It was a simple script that helped to automate the installation of Arch to relative perfection. To continue our path anology, this would be like an 8-lane highway next to an airport near a train station. People realized that there was a low barrier of entry to the OS market now that they could use arch as a starting point and then dress it up to their liking. This goal to be the personal use standard Linux distro has been achieved. Now their is fear that the team who earned the glory of Arch will be dethroned by a more exploitative competitor. Likely an adversary who attacks Arch directly, introduces proprietary technology, and can out develop/capitalize arch, would ultimately replacting or consuming them. As we have seen the race to simplification can also be rewarded that is why "arch-cels" cringe when Cachy users select a  window manager is a selection from a dropdown in a GUI durring setup. The choice is obfuscated by these abstactions. The user might not even know they can choose other options or older versions or just not use one, just like how customers at McDonalds do not think of the conditions of the animals they consume.  

Using Linux has become an annoying uber ride home from the airport. Maybe that is why people are not just forgetting how to drive but why they are forgetting to look outside.   

In my opinion Cachy is philsophically aligned with Arch as it helps to combine the great aspects of arch into a pre-congigured pacakge with GUI programs, desktop enviornemnts, window managers, compiler optimiazations, and thir own twists on the endless extensibility and customizability of Arch. and easy




# Commmand Line Interface
We will be interacting with the 

The command line can be found by pressing the windows (called the modification key in the linux world) and 


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