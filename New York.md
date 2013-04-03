Examples of citations within court decisions:

* 1301
* 130.10
* 723.00
* 104-A

Often preceded with "section ".

And citations within the Laws of New York:

* one hundred five-a, two hundred forty-a or three hundred ninety-six-a of this chapter (*seriously*)
* subdivisions one and two of section two hundred seven of this chapter
* section 1303 (Violations)
* section 1011 (Dissolution for failure to file certificate of type of Not-for-Profit Corporation Law under section 113)

WUT.

Section numbers are not unique -- they're reused between titles (or whatever they call their major sections.)

Each title has both a title ("Civil Service") and an three-character abbreviation ("CVS"), but it does not appear that the abbreviations are used in cross-references within the laws.

Here's a crude start:

```
((section\s)?)([0-9]{1,4})((\.[0-9]{1,4})?)((-[A-Z]{1})?)
```
