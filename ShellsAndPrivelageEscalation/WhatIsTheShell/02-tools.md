# Tools for Obtaining Shells

- **Shell Payload:** a malicious command to run
- We need a tool to send shell payloads, receive data, and interact with the shell

## Netcat

- The *swiss army knife* of networking.
- Usually preinstalled on many Linux distributions.
- Can do many network tasks
    - Banner grabbing
    - Receive reverse shells
    - Connect to bind shell ports
- Simple and common
- Often unstable by default.
- Stability can be improved

## Socat

- Advanced version of Netcat
- Usually more stable than Netcat shells.
- Two main drawbacks:
	- Syntax is harder.
	- Usually not installed by default on Linux systems.
- Workarounds for these issues exist
- Both Socat and Netcat also have `.exe` versions for Windows.

## Metasploit `multi/handler`

- Module path: `exploit/multi/handler`.
- Used to receive reverse shells.
- Best for controlled reverse shell handling.
- Gives more options for getting stable shells.
- Required for interacting with Meterpreter shells.
    - **Meterpreter Shells:** an advanced, dynamically extensible post-exploitation payload within the Metasploit Framework, commonly used by penetration testers to interact with a compromised host. Runs entirely in memory, injecting itself into a running process rather than creating new files on the disk, making it hard for traditional antivirus to detect
- Easiest way to handle staged payloads.

## Metasplout `Msfvenom`

- Part of the Metasploit framework tools.
- A payload generator.
- Distributed as a standalone tool.
- Used to generate payloads on the fly.
- Can generate many payload types
- Very powerful tool

## Kali Linux `/usr/share/webshells`
- A collection of webshells for ASP, ASPX, CFM, JSP, Perl, and PHP servers

## Helpful Shell Resources

- **PayloadsAllTheThings:** large collection of payload ideas.
- **PentestMonkey Reverse Shell Cheat Sheet:** popular quick reference.
- **SecLists:** while it is mainly used for wordlists, it also contains useful shell files.
