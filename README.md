# Cheat Sheet Personal
This repository serves as a quick reference of some useful commands.

**Replace 'pipe' by ➞ |**

## View, create, edit files and directories
| Command | Description |
| --- | --- |
| `touch` | Create a new empty file |
| `cat > [file]` | Create a new file with the text you type |
| `ln -s [path to be linked][path to create]` | Create a new file with the text you type |
| `$\n` | Line break - In Visual Code mark(.*) |

## Search for files and directories
| Command | Description |
| --- | --- |
| `find [directory] -name '[word]'` | Search for a file or directory based on exact name |
| `find [directory] -iname '[word]'` | Search for a file or directory based on name ignore case |
| `find [directory] -iname '[word]' -exec [command]` | Search for a file or directory based on name ignore case and execute a command |
| `grep -r [word-to-search-for] /path/to/directory/` | Search for a word or phrase in a series of files |

## Administration commands
| Command | Description |
| --- | --- |
| `sudo dnf install` | Install package on Red Hat based systems |
| `sudo dnf remove` | Remove package on Red Hat based systems |
| `reboot` | Reboot the system |
| `poweroff` | Shut down the system |

## Hard drive and storage
| Command | Description |
| --- | --- |
| `df -h` | Storage usage of mounted partitions |
| `tree` | View the directory structure for a path |
| `du` | See disk usage of directory's contens |
| `du -sh [path]` | Getting the Size of a Directory |
| `du -h [path] 'pipe' sort -rh 'pipe' head -5 ` | organize the 5 largest volumes |
| `lsof -i -P -n 'pipe' grep LISTEN ` | To see open ports |
| `lsof -i:[port]` | See a specific port |
| `sudo ps aux 'pipe' grep -i [word]` | Search process |
| `nslookup [host]` | Mapping between domain name and IP address |

## GIT
| Command | Description |
| --- | --- |
| `git config --global alias.[name][command]` | Create alias to commands |
| `git commit --amend -m "[new message]"` | Change message of last commit |
| Alias  | Command                                              | Description                        |
| gst    | `git status`                                         | Show the working tree status       |
| gl     | `git pull`                                           | Fetch from and integrate with remote |
| gp     | `git push`                                           | Update remote refs                 |
| gd     | `git diff`                                           | Show changes between commits/files |
| gau    | `git add --update`                                   | Add updated files to the index     |
| gc     | `git commit -v`                                      | Commit with verbose output         |
| gca    | `git commit -v -a`                                   | Commit all changes with verbose    |
| gb     | `git branch`                                         | List, create, or delete branches   |
| gba    | `git branch -a`                                      | List all branches                  |
| gco    | `git checkout`                                       | Switch branches or restore files   |
| gcob   | `git checkout -b`                                    | Create and switch to a new branch  |
| gcot   | `git checkout -t`                                    | Checkout and track a remote branch |
| gcotb  | `git checkout --track -b`                            | Create and track a new branch      |
| glog   | `git log`                                            | Show commit logs                   |
| glogp  | `git log --pretty=format:"%h %s" --graph`            | Pretty log with graph              |

## Network
| Command | Description |
| --- | --- |
| `netstat -pnat [port] 'pipe' grep [port]` | Id from port and ip connection |
| `nmap -sS -O 127.0.0.1` | Change message of last commit |
| `telnet [host][port]` | Status connection |

## Kubernetes (K8S)
| Command | Description |
| --- | --- |
| `kubectl create deployment [name]` | Create deployment |
| `kubectl edit deployment [name]` | Edit deployment |
| `kubectl delete deployment [name]` | Delete deployment |
| `kubectl get nodes ` | Status of differents K8S components |
| `kubectl get pod` | Status of differents K8S components |
| `kubectl get servies` | Status of differents K8S components |
| `kubectl get replicaset` | Status of differents K8S components |
| `kubectl get deployment` | Status of differents K8S components |
| `kubectl logs [pod name]` | Log to console |
| `kubectl exec -it [pod name] --bin/bash` | Get interactive terminal |
| `kubectl apply -f [path file]` | Apply a configuration file |
| `kubectl delete -f [path file]` | Delete with configuration file |
| `kubectl get configmap -n [name]` | Create component in a Namespace |
| `kubectl get configmap -o yaml` | Get yaml configuration |
| `kubectl create namespace [name]` | Create namespace|
