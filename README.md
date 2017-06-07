## Block malicious sites at DNS level with [unbound](http://www.unbound.net/)!
This repository is maintained by [k0nsl](https://k0nsl.org/blog/) ([i.am@k0nsl.org](mailto:i.am@k0nsl.org)) and is curated from four different sources apart from my own manual insertions.

* Instructions
    1. curl/wget/paste [this file](https://raw.githubusercontent.com/k0nsl/unbound-blocklist/master/blocks.conf) as `blocks.conf` and place it in
    `/usr/local/etc/unbound/` as `blocks.conf`
    2. nano `/usr/local/etc/unbound/unbound.conf`
    3. jump to line 482 (or EOF)
    4. add an include for "blocks.conf", e.g `include: "/usr/local/etc/unbound/blocks.conf"`

Presto! You’re done :^)

### Help

If you need any help you can contact me on IRC: https://webirc.k0nsl.ru