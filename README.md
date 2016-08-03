## Block malicious sites at DNS level with [unbound](http://www.unbound.net/)!##
This repository is maintained by [k0nsl](https://k0nsl.org/blog/) ([i.am@k0nsl.org](mailto:i.am@k0nsl.org))

**Instructions:**

 1. curl/wget/paste [this file](https://raw.githubusercontent.com/k0nsl/unbound-blocklist/master/blocks.conf) as `blocks.conf` and place it in
    `/usr/local/etc/unbound/`
 2. nano `/usr/local/etc/unbound/unbound.conf`
 3. jump to line 449
 4. add an include for "blocks.conf"

Presto! You’re done :^)
