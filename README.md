# check_joan
monitor [joan displays](https://getjoan.com/) plugin for Nagios

#### Usage:
`check_joan.sh -H http://joan_host:port -k api_key -s api_secret [-c <critical>] [-w <warning>]`

#### Options:
- -H  joan server url,
- -w  battery warning level (default 15%),
- -c  battery critical level (default 5%),
- -k  api key,
- -s  api secret,\
      can have prefix "file:" followed by location of the file with the secret.
- -u  show uuids in the output

#### Example:
`check_joan.sh -H http://joan.company.com:8081 -k d4508ad5491f14df -s file:etc/joan.secret`
