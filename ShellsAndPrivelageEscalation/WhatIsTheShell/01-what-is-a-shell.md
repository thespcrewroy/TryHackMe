# What Is a Shell?

- **Shell:** a program that lets us use a command-line interface (CLI).
- Common Linux shells: `bash`, `sh`.
- Common Windows shells: `cmd.exe`, `PowerShell`.

## Why This Matters in Pentesting

- Sometimes a vulnerable app on a server can be forced to run our commands.
- If that works, we can try to get shell access on the target machine.

## Two Main Shell Types

- **Reverse Shell:**
	- The target machine connects back to us.
	- We receive command-line access from that connection.
- **Bind Shell:**
	- The target machine opens a port.
	- We connect to that open port to run commands.
