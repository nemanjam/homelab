# Samba Docker

### Tutorial

- https://www.youtube.com/watch?v=2zZ3_1GRWrM
- https://github.com/dperson/samba

### docker-compose.yml examples

- https://shfahimi.net/2020/07/04/setting-up-your-home-media-server-2/
- https://naumann.dev/books/docker/page/samba
- http://idlesong.github.io/tech_life/2021/09/18/docker-server-on-pi.html

### Get all IPSs in LAN

- https://stackoverflow.com/questions/13669585/how-to-get-a-list-of-all-valid-ip-addresses-in-a-local-network
- https://www.dnsstuff.com/scan-network-for-device-ip-address

```bash
# nmap
sudo apt-get install nmap

nmap -sn 192.168.1.0/24

# ifconfig
arp -a
```

### Test LAN speed between 2 hosts

- https://phoenixnap.com/kb/linux-network-speed-test

```bash
sudo apt install iperf

# run server on port 5001
iperf -s

# run client
iperf -c 192.168.56.101
```

