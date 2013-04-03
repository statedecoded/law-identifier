Michigan court rulings' citations are fairly consistent.  They all are prefixed with "MCL ". (Not to be confused with "MCR" (Michigan Court Rules) or "MCE" (Michigan Rules of Evidence), which are not laws, but rules established by the court system.)

Here are some of the ways that I can find them used, both in court decisions and in cross-references within the MCL:

* MCL 600.1060 to 600.1082
* MCL 257.732
* MCL 750.160b
* MCL 324.76101

```
MCL\s([0-9]{1-3})\.([0-9a-z]{1-5})([a-z]?)
```

Michigan's section identifiers always have a decimal. Only one digit needs to exist on either side of the decimal. The first half of the identifier is the chapter number, the second is the section number. I have not identified any section identifier with more than five decimal digits, although some come precariously close (e.g., § 324.99921).

Because any decimal-bearing number would be matched, it's probably best to match with 
