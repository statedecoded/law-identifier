California doesn't have unique section identifiers—the portion of the code (e.g., "Penal Code") must be specified prior to the section identifier in order to make a match. That is to say that same section numbers are reused in multiple "Codes," so knowing "section 8001" doesn't tell you much.

Here are some of the ways that sections are cited within California Supreme Court decisions:

* Penal Code section 1538.5
* Code of Civil Procedure sections 377.20, 377.30, and 377.34
* section 1237.5
* sections 667.61, 12022 and 12022.3
* § 1203
* §6601.3
* §§ 1025, 1158

Those section identifiers lacking "Code" prefixes are within passages in which it is either stated explicitly at the outset which code they refer to (e.g. "all further statutory references are to the Penal Code unless otherwise indicated"), while in other cases it would be clear to a reader, but not inferable via machine.

Find citations:

```
([A-Za-z]+)\sCode\s(&#167;|section|sections)(\s?)([0-9]{1})([0-9\.]*)
```