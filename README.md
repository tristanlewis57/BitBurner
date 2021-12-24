# BitBurner
Collections of scripts used in bitburner

Control

Used on home (or anywhere you'd like to use it) to write actions to ports which will be read(peeked) by the zombie scripts

Use: run Control.ns hack/grow/weaken server

Zombie

Runs on hacked servers. Executes whatever action is written to the port at the time. If a new action is written to the port, it will finish the current action before starting a new one. This script just needs to be run on a server with as many threads as you want to use(Max threads is free GB/2).(As of now, all zombie scripts will stop running if they are not able to complete the action, so make sure there are no typos and your hacking level is high enough to hack)

ZBite

Run this to scan all servers and copy Zombie.ns to them. All servers with Zombie.ns will be added to a text file named zombies.txt(This does not run Zombie.ns)

Uprising

Run this with your available port hacks as an argument. This will root all rootable machines and run Zombie.ns(Zombie.ns will automatically close if it is not able to complete the command given by Control.ns or if there is no command available)

Zombification

Automatically sends commands to zombies to weaken/grow/hack a target. Priority of commands is min security level(weaken) > max money(grow) > hack. Very basic logic, but we are commanding zombies after all.

Use: run Zombification.ns server
