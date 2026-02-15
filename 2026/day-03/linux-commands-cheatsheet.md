# Process Management Commands:
| Command                   | Usage (One-line description)                     |
| ------------------------- | ------------------------------------------------ |
| `ps aux`                  | Show all running processes with detailed info    |
| `top`                     | Real-time view of system processes and CPU usage |
| `htop`                    | Interactive process viewer (enhanced top)        |
| `kill <PID>`              | Terminate a process by PID                       |
| `kill -9 <PID>`           | Force kill a process                             |
| `pkill <name>`            | Kill processes by name                           |
| `bg`                      | Resume a suspended job in background             |
| `fg`                      | Bring background job to foreground               |
| `jobs`                    | List active jobs in current shell                |
| `nice -n 10 <cmd>`        | Start a process with adjusted priority           |
| `renice <priority> <PID>` | Change priority of running process               |
| `uptime`                  | Show system uptime and load average              |

# File System Commands:
| Command                 | Usage (One-line description)                 |
| ----------------------- | -------------------------------------------- |
| `ls -la`                | List files with permissions and hidden files |
| `cd <dir>`              | Change directory                             |
| `pwd`                   | Show current directory path                  |
| `mkdir <dir>`           | Create a new directory                       |
| `rm -rf <dir>`          | Remove directory recursively                 |
| `cp -r src dest`        | Copy files/directories recursively           |
| `mv src dest`           | Move or rename files                         |
| `touch file.txt`        | Create empty file                            |
| `cat file.txt`          | Display file contents                        |
| `less file.txt`         | View file page by page                       |
| `head -n 10 file`       | Show first 10 lines of file                  |
| `tail -f file`          | Monitor file in real-time                    |
| `find /path -name file` | Search file by name                          |
| `chmod 755 file`        | Change file permissions                      |
| `chown user:group file` | Change file ownership                        |
| `df -h`                 | Show disk space usage                        |
| `du -sh folder`         | Show folder size                             |
| `mount`                 | Display mounted file systems                 |

# Networking & Troubleshooting:
| Command                   | Usage (One-line description) |
| ------------------------- | ---------------------------- |
| `ping google.com`         | Check connectivity to a host |
| `ip addr`                 | Show IP address information  |
| `curl http://example.com` | Fetch data from URL          |
| `dig google.com`          | DNS lookup for domain        |
| `netstat -tuln`           | Show listening ports         |
| `ss -tuln`                | Display socket statistics    |
| `traceroute google.com`   | Show packet path to host     |
| `hostname -I`             | Show system IP address       |
| `wget <url>`              | Download file from internet  |
| `nslookup domain.com`     | Query DNS information        |