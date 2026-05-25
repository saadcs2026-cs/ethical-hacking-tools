🔍 Maigret — The Deep Username Hunter

Sherlock's more powerful big brother.


What is Maigret?
Maigret is a free, open-source OSINT tool that hunts usernames across 500+ sites and collects detailed information about the person including accounts, photos, bios, and linked profiles.
Named after the famous French detective — Jules Maigret.

Maigret vs Sherlock
FeatureMaigretSherlockSites covered500+300+Collects profile data✅❌Photos & bios✅❌HTML/PDF reports✅❌Linked accounts✅❌

Installation
bash# Via pip
pip3 install maigret

# Via git
git clone https://github.com/soxoj/maigret
cd maigret
pip3 install -r requirements.txt

All Commands
bash# Basic search
maigret username

# Generate HTML report
maigret username --html

# Generate PDF report
maigret username --pdf

# Generate JSON report
maigret username --json

# Search specific site
maigret username --site twitter

# Increase sites checked
maigret username --top-sites 500

# Search multiple usernames
maigret user1 user2 user3

# Use proxy
maigret username --proxy http://127.0.0.1:8080

# Verbose output
maigret username --verbose

Sample Output
[+] Twitter      https://twitter.com/username     ✓ Found
[+] GitHub       https://github.com/username      ✓ Found
[+] Instagram    profile data collected           ✓ Found
[+] Reddit       post history found               ✓ Found
[-] TikTok       https://tiktok.com/@username     ✗ Not Found

Search completed. Found 47 accounts.
Report saved to: username.html
