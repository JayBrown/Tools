![Tools-platform-macos](https://img.shields.io/badge/platform-macOS-lightgrey.svg)
![Tools-code-shell](https://img.shields.io/badge/code-shell-yellow.svg)
[![Tools-license](http://img.shields.io/badge/license-MIT+-blue.svg)](https://github.com/JayBrown/Tools/blob/master/license.md)

# Command Line Tools: ipfg <img src="https://github.com/JayBrown/Tools/blob/master/img/jb-img.png" height="20px"/>
```
ipfg 1.1.1 (10-2017)
IPFS public gateway checker (extended cli version)

Running ipfg without an option will check the online status of all available IPFS gateways.
When using multiple options, only the final option will be recognized.

OPTIONS:
	-a | --add <URL>
		Add specified gateway URLs to local list (format: http[s]://<domain>.<tld>/ipfs/:hash)

	-d | --delete [<URL> | all]
		Delete specified or all gateway URLs from local list (format: see above)

	-h | --help
		This help page

	-l | --list [raw] [all | local | remote]
		Display listed gateways as domains or raw URLs

	-L | --local
		Only check gateways on local list

	-M | --manual <URL>
		Check only the specified URLs

	-R | --remote
		Only check gateways on remote list

	-s | --save | --backup
		Save remote gateway list to a local backup file

	-V | --version
		Print version number

	-w | --web
		Open web version of the IPFS public gateway checker

Copyright 2017 by Joss Brown (pseud.): https://github.com/JayBrown
License: MIT

Inspired by the original web-based IPFS Public Gateway Checker
https://github.com/ipfs/public-gateway-checker
```
