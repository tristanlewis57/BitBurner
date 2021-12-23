# BitBurner
Collections of scripts used in bitburner

CONTROL
Used on home (or anywhere you'd like to use it) to write actions to ports which will be read(peeked) by the zombie scripts
Use: run Control.ns hack/grow/weaken server

ZOMBIE
Runs on hacked servers. Executes whatever action is written to the port at the time. If a new action is written to the port, it will finish the current action before starting a new one. This script just needs to be run on a server with as many threads as you want to use.
