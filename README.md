# ssh-me
A simple script for sshing into your servers by server name

## Usage
```
./ssh_me server_name
```

## Configuration
The script contains an associative array called `servers` that maps server names to theri corresponding IP addresses. Please update this with your server names and IPs

declare -A servers=(
    ["web-01"]="192.168.41.12"
    ["web-02"]="4.5.6.32"
    ["lb-01"]="1.2.3.4"
)

## SSH key
I assume you, like me are using ssh key-based authentication. Update `~/.ssh/school` with the path to the private key
