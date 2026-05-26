# Maigret — The Deep Username Hunter

Sherlock's more powerful big brother.

## What is Maigret?
Maigret is a free open-source OSINT tool that hunts
usernames across 500+ sites and collects detailed
information including accounts, photos, bios, and links.

## Maigret vs Sherlock
Sherlock  → finds if account exists
Maigret   → finds account + full profile data,
             photos, connections, linked accounts

## Installation
pip3 install maigret

OR via git:
git clone https://github.com/soxoj/maigret
cd maigret
pip3 install -r requirements.txt

## Commands
maigret username                    basic search
maigret username --html             HTML report
maigret username --pdf              PDF report
maigret username --json             JSON report
maigret username --top-sites 500    search 500 sites
maigret username --site twitter     specific site only
maigret user1 user2                 multiple usernames

## Sample Output
[+] Twitter      found ✓
[+] GitHub       found ✓
[+] Instagram    found ✓
[-] TikTok       not found ✗
Found 47 accounts. Report saved.

## Use Cases
→ Hunt usernames across 500+ platforms
→ Build complete digital profiles
→ Find linked social accounts
→ Generate HTML/PDF reports
→ Deeper OSINT than Sherlock

"Sherlock finds the door. Maigret opens it."

⚠️ Only use on yourself or with permission.
