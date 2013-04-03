These are preceded by an initialism (ORS, for "Oregon Revised Statutes"), followed by a unique identifier comprised of a title number and a section number, separated by a period.

* ORS 18.455
* ORS 813.100, 813.140 or 813.150
* ORS 335.495 to 335.505

```
ORS\s([0-9]{1})([0-9A-Z]{0,3})\.([0-9]{3})
```

The `ORS\s` prefix can be omitted to yield a higher match rate and (anecdotally) a low rate of false matches. That said, many decimal-bearing numbers would be matched.
