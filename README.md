# REDIS-Monitoring-Scripts

One of the commericial products I work with uses [REDIS](http://redis.org) and I've developed a few scripts to help watch what is happening on the server between REDIS and the client.


##redis_connections

The script refreshes every 3 seconds and prints the current time and some basic connection info about how many sockets are in use to REDIS and how many connections REDIS has served since it's last restart.

It can be used to diagnose when the client is possibly misbehaving and opening up too many connections with out reusing them.
