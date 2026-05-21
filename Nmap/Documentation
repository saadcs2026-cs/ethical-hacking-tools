---What is Nmap?
Nmap (Network Mapper) is an open-source tool for network discovery and security auditing. 
It scans hosts, open ports, services, and OS details.


---Installation:

# Google Cloud Shell / Kali Linux
sudo apt install nmap -y

# From source (git)
git clone https://github.com/nmap/nmap.git
cd nmap
./configure && make && sudo make install

# Verify
nmap --version


---Basic Syntax:
nmap [options] [target]


---Host Discovery
nmap -sn 192.168.1.0/24       # Ping scan (no port scan)
nmap -Pn target                # Skip ping, scan anyway(bypass firewall)
nmap -PS target                # TCP SYN ping(check if device is responding)
nmap -PA target                # TCP ACK ping(Complete handshake between devices)


---Port Scanning
nmap target                    # Scan 1000 common ports
nmap -p 80 target              # Specific port
nmap -p 80,443,22 target       # Multiple ports
nmap -p 1-65535 target         # All ports
nmap -p- target                # All ports (shortcut)
nmap --top-ports 100 target    # Top 100 ports


---Scan Types
nmap -sS target    # SYN scan (stealth, default)
nmap -sT target    # TCP connect scan
nmap -sU target    # UDP scan
nmap -sA target    # ACK scan(send incomplete signal)
nmap -sF target    # FIN scan
nmap -sX target    # Xmas scan
nmap -sN target    # Null scan


---Service & Version Detection
nmap -sV target                          # Detect service versions
nmap -sV --version-intensity 9 target    # Max intensity
nmap -O target                           # OS detection
nmap -A target                           # All (OS + version + scripts + traceroute)


---Speed / Timing
nmap -T0 target    # Paranoid (slowest, stealthiest)
nmap -T1 target    # Sneaky
nmap -T2 target    # Polite
nmap -T3 target    # Normal (default)
nmap -T4 target    # Aggressive
nmap -T5 target    # Insane (fastest)


---NSE Scripts
nmap --script=default target              # Default scripts
nmap --script=vuln target                 # Vulnerability scan
nmap --script=http-title target           # Get page titles
nmap --script=ftp-anon target             # Check anonymous FTP
nmap --script=ssh-brute target            # SSH brute force test
nmap --script=all target                  # Run all scripts


---Output Formats(save results)
nmap target -oN output.txt    # Normal text
nmap target -oX output.xml    # XML
nmap target -oG output.grep   # Greppable
nmap target -oA output        # All formats at once
