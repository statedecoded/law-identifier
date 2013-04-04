Some example citations:

* 3.46.015
* 57.90.100
* 71A.10.910
* 35.102.900
* 35.32A.900

Three segments, separated by periods. The first segment is numeric, but may have an alpha suffix, one to three characters in all. The second is numeric, but may have an alpha suffix, two to four characters in all. And the third is numeric, always three digits.

```
([0-9]{1,2})([A-Z]?)\.([0-9]{1,3})([A-Z]?)\.([0-9]{1,3})
```

More accurate matches will result from using a prefix of `RCW\s`, but the structure of the identifiers is unusual enough that overbroad matches are not likely.
