Examples of section identifiers:

* Sec. 53.033
* Sec. 52.0165
* Sec. 3151.101
* Art. 7621f
* Art. 7808
* Sec. 4A.101

(Often "Section," sometimes "Sect." )

So there are article, and sections. I have no idea what the difference is—they seem to be used interchangeably.

In court opinions, citations appear as:

* Tex. Nat. Res. Code § 61.011
* Tex. Nat. Res. Code § 61.011, .0161
* Tex. Civ. Prac. & Rem. Code § 41.001
* Tex. Prop.Code Ann. §§ 21.015-.015
* Tex. Educ. Code § 21.307

Note that "Prop.Code" is not a typo. That style was employed repeatedly.

On second use, the major identifer is omitted, and replaced with "Id."

Here's a PCRE that should work for the identifiers as used within the Texas Statutes:

```
(Sec\.|Section|Art\.|Article)\s([0-9]{1})([0-9a-z]{0,4})(\.([0-9]{0,4})?)
```

That requires a proper prefix, though—it won't detect citations without them. (That's because literally any number that's at least two digits would qualify under that PCRE, lacking the prefix.) The citation must start with a single digit, and then can have up to four more letters and/or numbers. As a final, optional, component, there can be a period followed by 0–4 digits.

And here's a PCRE that should work for the identifiers as used within state court opinions:

```
Tex.\s([A-Za-z&\. ]+)\sCode\s§\s([0-9]{1})([0-9a-z]{0,4})(\.([0-9]{0,4})?)
```

The one catch is that it doesn't catch any of `Tex. Prop.Code Ann. §§ 21.015-.015` because of the presence of "Ann. ". The inclusion of that needs to be permissible.
