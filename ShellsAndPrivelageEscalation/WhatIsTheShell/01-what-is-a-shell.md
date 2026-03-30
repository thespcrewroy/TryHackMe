# What Is a Shell?

- A shell is a program that lets us use a command-line interface (CLI).
- Common Linux shells: `bash`, `sh`.
- Common Windows shells: `cmd.exe`, `PowerShell`.

## Why This Matters in Pentesting

- Sometimes a vulnerable app on a server can be forced to run our commands.
- If that works, we can try to get shell access on the target machine.

## Two Main Shell Types

- Reverse shell:
	- The target machine connects back to us.
	- We receive command-line access from that connection.
- Bind shell:
	- The target machine opens a port.
	- We connect to that open port to run commands.

## What This Room Covers

- Detailed explanation of both reverse and bind shells.
- Mostly theory and examples (code blocks + screenshots).
- Two practice VMs near the end:
	- One Linux VM
	- One Windows VM
- Practice questions are available in Task 13.

## Quick Summary

- Shell = command-line access.
- In exploitation, gaining a shell is often the first useful foothold.
- You will learn both ways to get shell access: reverse and bind.
