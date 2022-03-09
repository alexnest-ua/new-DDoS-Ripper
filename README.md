# DRipper

DESCRIPTION
-----------

This is an optimized version of DRipper.
Here is original code: https://gist.github.com/scamp/33807688d0ebdcfbd4c29a4b992a8b54,
you can see there a lot of cons like extra requests to Facebook and validator.w3.com,
trying establishing connection with attacked resource (but there is no need in it if you want to send a UDP packet).
Also, the old version is inefficient: you need run several processes to have your processor busy.

## Usage

```bash

██████╗ ██████╗ ██╗██████╗ ██████╗ ███████╗██████╗
██╔══██╗██╔══██╗██║██╔══██╗██╔══██╗██╔════╝██╔══██╗
██║  ██║██████╔╝██║██████╔╝██████╔╝█████╗  ██████╔╝
██║  ██║██╔══██╗██║██╔═══╝ ██╔═══╝ ██╔══╝  ██╔══██╗
██████╔╝██║  ██║██║██║     ██║     ███████╗██║  ██║
╚═════╝ ╚═╝  ╚═╝╚═╝╚═╝     ╚═╝     ╚══════╝╚═╝  ╚═╝

It is the end user's responsibility to obey all applicable laws.
It is just like a server testing script and Your IP is visible.

Please, make sure you are ANONYMOUS!
     
Usage: python DRipper.py [options] arg

Options:
  -h, --help            show this help message and exit
  -p PORT, --port=PORT  port (default: 80)
  -t THREADS, --threads=THREADS
                        threads (default: 100)
  -r RANDOM_PACKET_LEN, --random_len=RANDOM_PACKET_LEN
                        Send random packets with random length (default: 1
  -l MAX_RANDOM_PACKET_LEN, --max_random_packet_len=MAX_RANDOM_PACKET_LEN
                        Max random packets length (default: 48)
  -m ATTACK_METHOD, --method=ATTACK_METHOD
                        Attack method: udp (default), http
  -s HOST, --server=HOST
                        Attack to server IP

Example: python DRipper.py -s 192.168.0.1 -p 80 -t 100
```

## How to Run

Ensure you have Python 3 installed. Then clone this repo and run DRipper.py with params you need

```bash
git clone https://github.com/alexmon1989/russia_ddos.git
cd russia_ddos

# run
python DRipper.py -s 127.0.0.1 -p 80 -t 100 -r 1 -m udp
# OR
python3 DRipper.py -s 127.0.0.1 -p 80 -t 100 -r 1 -m udp
```

# License

This project is distributed under the MIT License, see [LICENSE](./LICENSE) for more information.
