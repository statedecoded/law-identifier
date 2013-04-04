Wyoming's citations are quite consistent. In a (small) corpus of court decisions, sections are always preceded with `§ `, and are often preceded with a specification that it's the Wyoming statutes to which they're referring. These are all valid citations in court decisions:

* Wyo. Stat. § 20-2-113
* WYO. STAT. § 20-2-113
* Wyo. Stat. Ann. § 20-2-204
* § 34-14-208 

Here are some samples from the Wyoming Statutes:

* 6-10-301
* 

So that structure is Title-Chapter-Section. It looks like identifiers are always numeric, never have suffixes, and never have decimals.

Here's a regular expression that captures things well enough:

```
((§\s)?)([0-9]{1,4})-([0-9]{1,3})-([0-9]{1,4})
```
