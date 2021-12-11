The three methods covered in this tutorial are:

* **rc.local** - Likely the easiest and simplest way to get your program to run on boot. The downside is that tasks started with rc.local happen before the X windows system starts, which means you will not have access to graphical user interface (GUI) elements.
* **autostart** - Used to automatically run your programs once LXDE (graphical desktop environment used by Raspbian) starts. It's slightly more complicated than rc.local, but it lets you run programs that require graphical elements.
* **systemd** - The new and popular way to automatically start programs in Linux. It is definitely the most complicated of the three, but it allows you to run before LXDE starts, wait until you have access to other processes (e.g. networking, graphical desktop), or simply restart your program over and over again until it works. As such, it is a robust way to create and manage services that run in the background.

via https://learn.sparkfun.com/tutorials/how-to-run-a-raspberry-pi-program-on-startup/all