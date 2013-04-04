Examples as found within the Oklahoma Statutes:

* §57-1
* §57-4.1
* §57-16a
* §57-509.1
* §27A-1
* §27A-1-1-102
* §27A-2-10-103
* §27A-3-2-106b
* Rule 257:1-1-1

Cross-references as found within the Oklahoma Statutes:

* Section 988.12 or 991a-2 of Title 22
* Section 980 of Title 22 of the Oklahoma Statutes
* Section 192 of Title 74 of the Oklahoma Statutes

Clearly, two different regular expressions are going to be needed here. First, one to pick up non-xref citations:

```
(((§(\s?))?)|(Rule\s))([0-9]{1,3})((:?)([0-9A-Z]{1})?)-([0-9]{1,3})([a-z]?)((\.[0-9]{1,2})?)((-[0-9]{1,2})?)((-[0-9]{1,3})?)([a-z]?)
```

Then, one to pick up cross-references:

```
Section\s([0-9a-z\.-]{1,6})\sof\sTitle\s([0-9]{1,3})
```

Both of those are going to need a lot more testing.
