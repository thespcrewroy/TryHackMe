# Tools for Getting Shells (Simple Notes)

- To get shells, we need:
	- Shell payload/code (malicious command to run)
	- A tool to send/receive and interact with the shell

## Netcat

- Known as the "Swiss Army knife" of networking.
- Can do many network tasks (for example, banner grabbing).
- In this room, it is mainly used to:
	- Receive reverse shells
	- Connect to bind shell ports
- Netcat shells are often unstable by default.
- Stability can be improved (covered later).

## Socat

- Similar to Netcat, but more powerful.
- Socat shells are usually more stable than Netcat shells.
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
