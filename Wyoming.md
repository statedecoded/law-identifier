Wyoming, on the other hand, is much more consistent. In their (admittedly small) corpus, sections are always preceded with `§ `, and often preceded with a specification that it's the Wyoming statutes to which they're referring. These are all valid citations:

*Wyo. Stat. § 20-2-113
*WYO. STAT. § 20-2-113
*Wyo. Stat. Ann. § 20-2-204
*§ 34-14-208 

Here's a regular expression that captures things well enough:

```
&#167;(\s?)([0-9]{1,4})-([0-9]{1,3})-([0-9]{1,4})
```

This corpus is too small to generate meaningful numbers regarding the accuracy of this PCRE.