## Per Kevin Finisterre (not TBS) OpenPilot is what you *SHOULD* be using. ;)

 I (Kevin Finisterre) do not specifically condone TauLabs in general, nor do I support 'Quanton' as a body of work. 
 (This has NOTHING to with Team Black Sheep or sirperna at ALL, as I am NOT affiliated with them)

 The FPVLab thread "Announcing the TBS GEMINI fpv racer / mini hex" is the thread that houses this *product*
 http://fpvlab.com/forums/showthread.php?32545-Announcing-the-TBS-GEMINI-fpv-racer-mini-hex

 Please be aware that TauLabs attempted to prevent this product from making use of the TauLabs GCS. Internal conversations
 were had over kfinisterre's involvement as being a reason to *block* a pull request to include Colibri Flight Controller

 After some pressure from Team Black Sheep, TauLabs caved a bit and at least added the USB ID to the "Development Hardware" page. 
 https://github.com/TauLabs/TauLabs/wiki/Development-Hardware-IDs
 Colibri	0x91	0x01	0x20a0	0x4235

 At this point in time the product is not *officially* supported by TauLabs. The "Open Source" nature of the project remains questionable

 Colibri is a clone of Quanton which is a clone of Revo which is VERY touchy in the community. 
 In jest even R_Lefebvre chimed in on the concept well before Colibri existed. See the Quanton post on DIYDrones - http://diydrones.com/profiles/blog/show?id=705844%3ABlogPost%3A1110560&commentId=705844%3AComment%3A1227209&xg_source=activity
 "Wow, clone of a clone.  $30.  If somebody makes a clone of a clone of a clone, will it be $3? ;)"

 The MAIN reason I chose to engague in this was the snarky attitude presented by guilhermito when perna asked for help.

 "Re: New Tiny Hardware
 by Perna » Mon Apr 07, 2014 1:58 pm

 I looking for somebody who can help me make a new hardware ID for the 
 board with an own hardware name and to make the GCS recognize it with a 
 own picture."
 
 "Re: New Tiny Hardware
  by guilhermito » Mon Apr 07, 2014 3:07 pm
 
 Good luck :)"
  
 It just didn't seem very 'Neighborly' see FYN-FYTN protocol https://www.youtube.com/watch?v=TbiMZMd7v4g

![Colibri Preview](http://i.imgur.com/ymF4UOS.jpg)
![Colibri2 Preview](http://i.imgur.com/N6ziuIN.jpg)
![Colibri3 Preview](http://i.imgur.com/CozeIwj.png)

 These files are provided out of courtesy to an acquantence that I met while reading about new hardware that would support TauLabs (and OpenPilot by proxy) 
 I am doing this patch primarily as an exercise to help me continue my understanding of OpenPilot based software and hardware interactions

 This topic originated on the PhoenixPilot Google Group - https://groups.google.com/forum/!topic/phoenixpilot/IK5sjLUFU84
 The "New Tiny Hardware" topic was discussed briefly after which point one of my comments was deleted by the group administrator. 
 Remaining public conversations have been held on the TauLabs forum (which I am banned from) http://forum.taulabs.org/viewtopic.php?f=21&t=94
 Additional relevant notes here https://groups.google.com/forum/#!msg/phoenixpilot/xbcV8DGkznw/a4orL4pIgrYJ

 Tau Labs

## Goals
The goal of Tau Labs is to focus on writing high quality open source code for autopilots that can easily provide the basis for research projects or further development by anyone.  The project focuses on high quality code, robust testing, and ease of use. Our target audience is professionals, researchers, and students, but we want to make those more advanced techniques easy and accessible for anyone.

By “research”, we mean not only universities or institutions focused on research on UAVs, but any group who might have use for UAVs for their research purpose. Examples include UAVs used for agricultural surveys, air quality logging. By “students” we mean aiming the use of our project in the classroom, especially thanks to the availability of an entry-level reference platform (see below).

The Tau Labs software is released under the GPL and will be treated in that spirit.  The code was forked from the OpenPilot project in November of 2012.  Porting the software to new boards is encouraged and fun.  The project will also maintain a set of reference platforms which the code will be more frequently tested against and will be expected to perform optimally.  As it was put, these will receive “A+ development support.”  As Lilvinz put it, with open source you can only give and create and we want to continue doing that.

## Getting involved
Click that big fork button on github and start coding!  We use pull requests as reviews so expect a lot of constructive feedback!

In addition check out http://forums.taulabs.org for more discussion

Chat on freenode.net #taulabs

## Code Layout

Here is a quick breakdown of the main directories to get you oriented

* flight - contains the firmware components of the code
* flight/target - the location of the board targets (e.g. flight/targets/freedom)
* flight/PiOS - contains the drivers
* flight/Modules - the flight control logic, broken into modules that communicate via UAVObjects
* flight/tests - unit tests for some components of the flight code
* ground - contains the GCS code
* shared - contains UAV Object definitions shared between the GCS and the flight firmware
* androidgcs - contains the ground control software for android

