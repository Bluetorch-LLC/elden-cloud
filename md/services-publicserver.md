## Elden Cloud - Public Server
A tiny Alpine Linux server with bare minimum specs, that anyone can log into.
You may use the server for any ethical, low-bandwidth, low-demand activity.

This is basically an experiment to see if randos can cooperatively use a shitty
computer. If you have a genuine use for a few kbps of publicly-accessible
bandwidth, you probably have an even worse internet/hardware situation than me.

### Logging In
Download [this key](/files/pubserver.pem) and log in like so:
```
ssh-add ~/Downloads/pubserver.pem
ssh pub@elden.cloud -p 25699
```

### Specs (shared by all users)
- 1 thread on a shitty AMD APU from 2012
- 256MB of RAM
- 16GB disk image
- Ports 22700-22999 are open
- Basic utilities and a few scripting languages installed

### Rules
- Do not attempt to change `.zshrc` or `.ssh/authorized_keys`.
- Make one uniquely-named folder in the home, to hold your files. Do not
clutter the home with loose files. I will regularly log in and delete them.
- Follow the same practice as above with your tmux sessions. Name them with
`tmux new -s <name>`.
- Respect other users and their processes and data. But don't keep anything
vitally important here, either.
- Do not use the public server for any illegal or unethical activities.
- If you have any shred of Linux and/or networking knowledge, you'll find out
in three seconds that the server is bridged to my LAN. I don't particularly
give a shit if you look around, but don't try to disrupt my network.
- Abuse = block, reset, or shutdown.
