Oregon. These are formatted like Michigan's—preceded by an initialism (ORS, for "Oregon Revised Statutes"), followed by a unique identifier comprised of a title number and a section number, separated by a period.

* ORS 18.455
* ORS 813.100, 813.140 or 813.150

```
ORS\s([0-9]{1})([0-9A-Z]{0,3})\.([0-9]{3})
```

There are 1,373 matches for that PCRE.

This more liberal PCRE (eliminating the `ORS\s` prefix) finds an additional 83 matches (1,456 in all):

```
([0-9]{1})([0-9A-Z]{0,3})\.([0-9]{3})
```

Of those additional matches, 95.2% are proper references, with just four matches invalid. (Of those four, 3 are to the Uniform Trial Court Rules with numbers that actually resolve to the ORS, and 1 is just a number (8.000) that does not resolve to the ORS.)

Given the high rate of accuracy, I would use the more liberal PCRE, because that is, for my purposes, an acceptable trade-off.
