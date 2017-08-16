![Tools-platform-macos](https://img.shields.io/badge/platform-macOS-lightgrey.svg)
![Tools-code-shell](https://img.shields.io/badge/code-shell-yellow.svg)
[![Tools-license](http://img.shields.io/badge/license-MIT+-blue.svg)](https://github.com/JayBrown/Tools/blob/master/license.md)

# Command Line Tools: dies <img src="https://github.com/JayBrown/Tools/blob/master/img/jb-img.png" height="20px"/>
```
dies v1.0 (2017.08) by Joss Brown
Shell script utility to convert English to Latin weekday names

USAGE
	dies [-i | -s | -u | -v] <WEEKDAY>
	dies [-h | -V]

MAIN OPTIONS
	-i, --j2i
		Print 'I' instead of 'J', i.e. 'Iovis' instead of 'Jovis'

	-s, --short
		Print short-form names, e.g. 'Mar' instead of 'dies Martis'

	-u, --upper
		Print output in uppercase, e.g. 'DIES SOLIS' or 'MAR'

	-v, --u2v
		Print 'V' instead of 'U', e.g. 'SATVRNI' instead of 'SATURNI'
		This option is ignored in lowercase.

ADDITIONAL OPTIONS
	-h, --help
		This help page

	-V, --version
		Version number and release date

FORMATS
	Use the following conventions for the days of the week:
		Sunday | Sun. | Sun | Su | U | 0
		Monday | Mon. | Mon | Mo | M | 1
		Tuesday | Tues. | Tues | Tue. | Tue | Tu | T | 2
		et cetera

EXAMPLES
	dies 6
	dies -u Sunday
	dies -s -i Thu
	dies -u -i -v U M T W R F S
	dies $(date +%w)
	date -f '%Y %m %d' -j "1969 07 20" +%a | xargs -I {} dies -u -s -i -v {}

	Regarding numeral input, dies presupposes the %w option (GNU & BSD date) with Sunday as '0'

	To avoid the printing of negative results and errors, redirect stderr to /dev/null:
	dies <WEEKDAY> 2>/dev/null
```
