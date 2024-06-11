# efficient-makejail

Makejail to make some operations more efficient.

* Disable `sendmail(8)` to avoid running it.
* Add a root jitter of `60` seconds to `cron(8)`.
* Add `-ss` to `syslogd(8)`.

Example:

```
INCLUDE gh+DtxdF/efficient-makejail
INCLUDE gh+AppJail-makejails/hello
```

Run:

```
appjail makejail -j hello
```
