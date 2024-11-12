
# PrivNet: Privacy Network

PrivNet is an anonymization tool that configures iptables and Tor to route all services, traffic and DNS through the Tor network. This tool allows users to route internet traffic through Tor and hide their real IP address.

## Features
- Installing and removing iptables rules
- Connecting to the Tor network to get its IP address and geolocate it
- Changing circuit with a new IP
- Automatic IP change at a specified interval
- Fast and easy to use

## Installation
```shell
git clone https://github.com/Fujimori-Zeta/PrivNet.git` 
```
## Requirements

Before you can use PrivNet, you need to make sure that you have the necessary requirements installed. You can install these requirements by running the following command:

```shell
pip install -r requirements.txt
```

## Install Tor 

Before you can use PrivNet, first you need to install the tor package:

```shell
apt-get clean
apt-get update
apt-get upgrade 
apt-get install tor
```
## Getting Started

Run the following command to use the tool::

```shell
python3 privnet.py
```

### Options

- `-l` or `--load`: Tor installs iptables rules.
- `-f` or `--flush`: Flushes the iptables rules to default.
- `-r` or `--refresh`: Changes the circuit and gets a new IP.
- `-i` or `--ip`: Displays the current public IP address.
- `-a` or `--auto`: This option enables automatic IP change every X seconds
- `-t` or `--interval`: Interval for automatic IP change in seconds (default: 3600)


## About the Original Author

PrivNet is a fork of the original tool called toriptables2, which was created by [Rupe](https://github.com/ruped24). Rupe developed the initial version of the tool three years ago. However, the original tool was written in Python 2.7 and is no longer compatible with the latest versions. Therefore, this forked version, PrivNet, has been updated and modified to work with Python 3.
I would like to express my gratitude to Rupe for the inspiration and foundation provided by the original tool. Without his work, this updated version would not have been possible.
If you would like to learn more about the original tool, you can visit the [toriptables2 repository](https://github.com/ruped24/toriptables2).



## License
PrivNet is released under the MIT License. See LICENSE for more information.
