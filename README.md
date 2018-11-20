# Heka
A lightweight SSH honeypot for Unix/Linux

Heka spins up a temporary SSH server on a specified port and logs all SSH connections, outputting received username and password combinations to the screen as well as a log file.

This script is based around Paramiko, which is a Python (2.7, 3.4+) implementation of the SSHv2 protocol. It leverages a Python C extension for low level cryptography, but for all other aspects, it is a pure Python interface for SSH networking.

## Wiki:
 * [Setup instructions](https://github.com/apacketofsweets/Heka/wiki/Setup-instructions)
 * [Requirements](https://github.com/apacketofsweets/Heka/wiki/Requirements)
 * [Disclaimer](https://github.com/apacketofsweets/Heka/wiki/Disclaimer)
