# Pwnshodo
Pwnshodo adalah alat yang mengumpulkan semua subdomain yang tersedia untuk nama host atau organisasi tertentu dari Shodan. Alat ini dirancang untuk digunakan dari Penetration Tester dan Bug Bounty Hunters.

[!image](https://)

## Requirments/Install
 1. Shodan paid account.
 1. Python3

```
pip install shodan
pip install termcolor
shodan init YOUR_API_KEY
```

## Usage
You have 2 python scripts, the first one will search for your scope subdomains using 2 filters hostname and `Ssl.cert.subject.CN` The second script will search using filter org

 * **`pwnshodan_hostname.py`**
```sh
> scope_domains.txt example:
yahoo.com
uber.com
twitter.com

> Run: 
python3 pwnshodan_hostname.py scope_domains.txt
```
 * **`pwnshodan.py`**
```sh
> scope_organizations.txt example: 
Google LLC 
Uber Technologies LLC 
Twitter

> Run: 
python3 pwnshodan.py scope_organizations.txt
```
&copy; [pwnlaboratory](https://github.com/pwnlaboratory) [deb0con](https://github.com/deb0con) [andripwn](https://github.com/andripwn) 
