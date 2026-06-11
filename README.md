# This configuration has been tested in real time and works under any conditions.

# Sweet-spot-conf-for-wireguard-or-amneziaWG
[Interface]
# ⚠️ YOUR PRIVATE KEY - Don't share your real one
PrivateKey = YOUR_PRIVATE_KEY_HERE

# adress of proton vpn (you can use your own private ip too)
Address = 10.2.0.2/32, 2a07:b944::2:2/128

# DNS of AdGuard (fast and blocks ADs)
DNS = 94.140.14.14, 94.140.15.15, 2a10:50c0::ad1:ff

# MTU: the sweet spot for speed and stability
MTU = 1320

# AmneziaWG obfuscation parameters (anti-lock without loss of speed)
Jc = 5
Jmin = 50
Jmax = 1000
S1 = 32
S2 = 120
H1 = 1
H2 = 2
H3 = 3
H4 = 4

[Peer]
# Server public key US-FREE#3 (Miami)
(use your public key if you want)
PublicKey = bOz7aS+OtfmIiGLlQmnHrWb+wzw5qFp6PKdWPRlVORc=

# All traffic through the VPN
AllowedIPs = 0.0.0.0/0, ::/0

# Port 443: camouflage to avoid blockades (you can use your vps)
Endpoint = 195.181.163.1:443

# It keeps the connection active without wasting battery power.
PersistentKeepalive = 16
# if you use pure wireguard just delete the things of amneziaWG
