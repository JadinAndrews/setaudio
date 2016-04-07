# setaudio
A quick and dirty Pulse Audio Quality switcher. (For audiophiles who only care about audio fidelity)

# How to use this
- Download all files and extract into a working directory
- Open a terminal and run: chmod +x setaudio
- Then run:
-  ./setaudio -lq or -hq 
-  to load the lq.conf or hq.conf files into the pulseaduio configuration.

I don't really plan on maintaining this code much, but I will add a few more features to it.

If you would like to keep your old pulseaudio config, then please back it up or better, replace the lq.conf file with your current daemon.conf with the following command executed in the setaudio directory.
- cp /etc/pulse/daemon.conf ./lq.conf

# Why did I make this?
I just wanted a quick and easy way to change quality settings to see if they made any difference. It makes experimenting with different settings a bit quicker, as well as reverting to a less cpu intensive configuration with less pain.

# What do I still want to do?
I would 'like' to add a few sed and awks to remove the need for separate lq.conf and hq.conf files,
this way it would be possible to add setaudio to /usr/bin so that it could be executed anywhere.
Also, I think it could automatically back up the daemon.conf

Lastly, please use this at your own risk, it is a very simple script, but it does require some root privileges to do some things, so there is a possibility it could kill your machine.

Enjoy!
