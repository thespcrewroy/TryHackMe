# Tools for Obtaining Shells

- **Shell Payload:** a malicious command to run
- We need a tool to send shell payloads, receive data, and interact with the shell

## Netcat

- The *swiss army knife* of networking.
- Can do many network tasks
    - Banner grabbing
    - Receive reverse shells
    - Connect to bind shell ports
- Netcat shells are often unstable by default.
- Stability can be improved

## Socat

- Advanced version of Netcat
- Usually more stable than Netcat shells.
- Two main drawbacks:
	- Syntax is harder.
	- Usually not installed by default on Linux systems.
- Netcat is usually preinstalled on many Linux distributions.
- Workarounds for these issues exist (covered later).
- Both Socat and Netcat also have `.exe` versions for Windows.

## Metasploit `multi/handler`

- Module path: `exploit/multi/handler`.
- Used to receive reverse shells (like Netcat/Socat).
- Gives more options for getting stable shells.
- Required for interacting with Meterpreter shells.
- Easiest way to handle staged payloads.

## Msfvenom

- Part of the Metasploit framework tools.
- Distributed as a standalone tool.
- Used to generate payloads on the fly.
- Can generate many payload types, but this room focuses on reverse/bind shell payloads.
- Very powerful tool (covered more deeply later).

## Helpful Shell Resources

- PayloadsAllTheThings: large collection of payload ideas.
- PentestMonkey Reverse Shell Cheat Sheet: popular quick reference.
- Kali Linux often includes webshells at `/usr/share/webshells`.
- SecLists (mainly for wordlists) also contains useful shell-related files.

## Quick Summary

- Netcat: simple and common, but less stable.
- Socat: more stable and powerful, but harder syntax.
- `multi/handler`: best for controlled/stable reverse shell handling.
- Msfvenom: payload generator.
- Keep shell cheat sheets and payload repositories handy.
