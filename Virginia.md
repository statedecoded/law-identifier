```
([[0-9]{1,})([0-9A-Za-z\-\.]{0,3})-([0-9A-Za-z\-\.:]*)([0-9A-Za-z]{1,})
```

This is in use on [Virginia Decoded](http://vacode.org), with great success. The structure necessitates at least numbers separated by a hyphen, making overbroad matches uncommon, so this is best employed as written, without requiring a `§\s` prefix.
