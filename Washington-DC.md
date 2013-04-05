Example section numbers:

* § 9-812
* § 24-201.19
* § 24-211.01
* § 24-221.01a
* § 24-1105
* § 50-1505.03
* § 50-2201.04c
* § 29A-101.76

Structure is title-chapter/section. That is, the first segment is the title number, then a hyphen. The second segment is the chapter number followed by the section number. § 9-812, for example, is Title 9, Chapter 8, the 12th section.

This matches those example sections, optionally matching the section symbol:

```
((§\s)?)([0-9]{1,2})([A-Z]?)-([0-9]{3,4})((((\.)([0-9]{2}))?)([a-z]?))
```

It remains to a) test this without the `§\s` prefix to see if overbroad matching is a problem and b) write a PCRE for court rulings.
