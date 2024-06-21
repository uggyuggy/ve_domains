# .ve domain names

## 🎯 Purpose

This repository purpose is to daily share the list of `.ve` domain names. (As I have not found another public share of this list, including under SLDs, for now)


## ☕ Sample

```
$ curl -s -L https://github.com/uggyuggy/ve_domains/raw/main/ve.txt -o ve.txt
$
$ wc -l ve.txt 
23637 ve.txt
$
$ head ve.txt
# ve domain names extracted from nameservers on 21Jun2024 00:21 UTC
0800comercio.gob.ve.
0800rentahouse.com.ve.
0es3.com.ve.
1-and-1.com.ve.
1-y-1.com.ve.
1.com.ve.
1000rifas.com.ve.
100franquicias.com.ve.
100x100banc0.com.ve.
$
```


## 📰 Informations

- Data is retrieved using DNS "zone walking" method

- There is no garantee of anything (I hope the zone is "full".. but who knows except the registry ?)

- When writing this, I think there is both, some domains at the apex, and some under SLDs like `.com.ve.`, `.gob.ve.`, `.edu.ve.` ...


- You may be interested by some other "zone walked" TLDs.
Look into https://github.com/maaaaz/dnsdumps repo which provides others
(At date of this README, Thomas have only the `.ve.` domains at the Apex, not under SLDs)

- There are 23637 domain names (as the time of writing this page)

- The file served here should be updated 1 time per day to not overload the remote servers for no reason.

- The file contains an additional comment line at the top starting with `#` that contain an UTC date information.

- For now there is a single comment line, but in case I add more in the future, you may better remove everything that start with a `#`

- The domain names end with `.ve.` (Ending dot, as FQDN)

- The domain names are provided sorted ( `LC_ALL=C sort -u`)

- There are some IDN domains (`xn--)`

- If there is no domain list provided for a specific day, this could mean my script failed to build/push the list

- You should be able to guess if the file has been updated successfully by checking either:
  - The date into the first comment line. `LC_TIME=C date -u +'%d%b%Y %H:%M UTC'`
  - The date of the last Github commit


## 🚧 Todo

- [x] Write README
- [x] Add emojis to the README (very important 🚨)
- [ ] Inform maaaaz/dnsdumps/issues/1
- [ ] Add more warning notifications in case of script failures
- [ ] Add more control to guess if something went wrong with script
- [ ] After I will be confident it's running as expected, possibly informing https://github.com/jschauma/tld-zoneinfo/
- [ ] ...




