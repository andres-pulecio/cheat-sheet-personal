# cheat-sheet-personal
This repository serves as a quick reference of some useful commands.

**Replace 'pipe' by ➞ |**

## View, create, edit files and directories
| Command | Description |
| --- | --- |
| `touch` | Create a new empty file |
| `cat > [file]` | Create a new file with the text you type |
| `ln -s [path to be linked][path to create]` | Create a new file with the text you type |

## Search for files and directories
| Command | Description |
| --- | --- |
| `find [directory] -name '[word]'` | Search for a file or directory based on exact name |
| `find [directory] -iname '[word]'` | Search for a file or directory based on name ignore case |
| `find [directory] -iname '[word]' -exec [command]` | Search for a file or directory based on name ignore case and execute a command |

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
| `du -h [path] 'pipe' sort -rh 'pipe' head -5 ` | organize the 5 largest volumes |
| `lsof -i -P -n 'pipe' grep LISTEN ` | To see open ports |
| `lsof -i:[port]` | See a specific port |

## GIT
| Command | Description |
| --- | --- |
| `git config --global alias.[name][command]` | Create alias to commands |
| `git commit --amend -m "[new message]"` | Change message of last commit |

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
