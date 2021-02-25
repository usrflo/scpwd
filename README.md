# scpwd
secure copy pwd - quickly echo scp path including username@hostname and optional filename for productivity.

## Samples

```console
/etc/ $ scpwd
me@myserver.example.tld:/etc
/etc/ $ scpwd /opt/
me@myserver.example.tld:/opt
/etc/ $ scpwd my.conf
me@myserver.example.tld:/etc/my.conf
/etc/ $ scpwd /usr/local/etc/my.conf
me@myserver.example.tld:/usr/local/etc/my.conf
/etc/ $ scpwd ../usr/local/etc/my.conf
me@myserver.example.tld:/usr/local/etc/my.conf
```

## Optional user config file

The external username and hostname may differ from local settings.
Place a file named .scpwd in a user's home directory to override the locally determined user@hostname with
```
LOGIN=someuser@someproxy.example.tld
```

Florian Sager, sager@agitos.de, 2021-02-25, MIT license
