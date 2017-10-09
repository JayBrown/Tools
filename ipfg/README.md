![Tools-platform-macos](https://img.shields.io/badge/platform-macOS-lightgrey.svg)
![Tools-code-shell](https://img.shields.io/badge/code-shell-yellow.svg)
[![Tools-license](http://img.shields.io/badge/license-MIT+-blue.svg)](https://github.com/JayBrown/Tools/blob/master/license.md)

# Command Line Tools: ipfg <img src="https://github.com/JayBrown/Tools/blob/master/img/jb-img.png" height="20px"/>
```
ipfg 1.2.1 (10-2017)
IPFS public gateway checker (extended cli version)

Running 'ipfg' without an option will check the online status of all available IPFS gateways.

OPTIONS:
	-a | --add <URL>
		Add specified gateway URLs to local list

	-c | --compare
		Check remote gateway list for changes incl. auto-backup

	-d | --delete [<URL> | all]
		Delete specified or all gateway URLs from local list

	-h | --hash
		Print current and saved IPFS hashes incl. auto-backup

	-H | --help
		This help page

	-l | --list [raw] [all | local | remote]
		Display listed gateways as domains or raw URLs

	-L | --local [raw]
		Only check gateways on local list

	-M | --manual <URL>
		Check only the specified URLs

	-R | --remote [raw]
		Only check gateways on remote list

	-s | --save [all | hash | url]
		Manually save remote data to local backup files

	-u | --upload | --cache [local | remote] <URL>
		Cache an IPFS object from a local or remote node on a gateway node

	-V | --version
		Print version number (incl. update check)

	-w | --web
		Open web-based version of the IPFS public gateway checker

Adding 'raw' to a gateway check will print the full URL instead of the gateway domain.
When using multiple options, only the final option will be recognized.
Caching will only be attempted on one gateway at a time.

GATEWAY URL FORMAT:
	http[s]://<domain>.<tld>/ipfs/:hash

EXAMPLES:
	ipfg
	ipfg -M https://ipfs.io/ipfs/:hash
	ipfg -l remote
	ipfg -R raw
	ipfg -a https://mygateway.com/ipfs/:hash
	ipfg -l raw local
	ipfg -L
	ipfg raw
	ipfg -d https://mygateway.com/ipfs/:hash
	ipfg -u local https://ipfs.io/ipfs/"$(echo 'This is an ipfg cache run.' | ipfs add -Q)"

Copyright 2017 by Joss Brown (pseud.): https://github.com/JayBrown (License: MIT)

See also the web-based IPFS gateway checker: https://github.com/ipfs/public-gateway-checker
```
