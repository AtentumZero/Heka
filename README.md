# Heka
A lightweight low-interaction SSH honeypot for Unix/Linux

Heka spins up a temporary SSH server on a specified port and logs all SSH connections, outputting received username and password combinations to the screen as well as a log file. 

This script is based around Paramiko, which is a Python (2.7, 3.4+) implementation of the SSHv2 protocol. It leverages a Python C extension for low level cryptography, but for all other aspects, it is a pure Python interface for SSH networking.

## Benefits of Heka 
The main benefit of using Heka over monitoring genuine SSH logs to research bot behaviour or using higher interaction honeypots is that it will not allow an attacker to login - so while that limits you to only getting username and password details for the password attack, there shouldn't be a possibility of an attacker actually logging in to a genuine SSH instance. This is ideal for tracking the behaviour of botnets that use default username and passwords to login to system - e.g. Mirai and Wopbot.

That said however, if you're looking to monitor what kinda of exploit code attackers are using after successfully brute-forcing an SSH server, then Heka in its current state is not suitable. 

## Wiki:
 * [Setup instructions](https://github.com/apacketofsweets/Heka/wiki/Setup-instructions)
 * [Requirements](https://github.com/apacketofsweets/Heka/wiki/Requirements)
 * [Disclaimer](https://github.com/apacketofsweets/Heka/wiki/Disclaimer)
