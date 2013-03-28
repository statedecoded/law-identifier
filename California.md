I've spent some quality time with California's court rulings. This is a good worst-case example. California doesn't have unique section identifiers—the portion of the code (e.g., "Penal Code") must be specified prior to the section identifier in order to make a match. That is to say that same section numbers are reused in multiple "Codes," so knowing "section 8001" doesn't tell you much.

Here are some of the ways that sections are cited within California Supreme Court decisions:

* Penal Code section 1538.5
* Code of Civil Procedure sections 377.20, 377.30, and 377.34
* section 1237.5
* sections 667.61, 12022 and 12022.3
* § 1203
* §6601.3
* §§ 1025, 1158

Those section identifiers lacking "Code" prefixes are within passages in which it is either stated explicitly at the outset which code they refer to (e.g. "all further statutory references are to the Penal Code unless otherwise indicated"), while in other cases it would be clear to a reader, but not inferable via machine.

Here's a quick, flawed regular expression to find citations within the 110 2012 decisions:

```
([A-Za-z]+)\sCode\s(&#167;|section|sections)(\s?)([0-9]{1})([0-9\.]*)
```

That regular expression matches 572 citations, or an average of 5 per decision.

For comparison's sake, that the following regular expression has 7,292 matches, an average of 66 per decision:

```
(&#167;|section|sections)(\s?)([0-9]{1})([0-9\.]*)
```

Many states had no bulk downloads available, despite being listed in Court Listener, at least in the various years that I tried (generally 2009–2013), including Utah, Alaska, West Virginia, and Wisconsin.