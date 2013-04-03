California doesn't have unique section identifiers—the portion of the code (e.g., "Penal Code") must be specified prior to the section identifier in order to make a match. That is to say that same section numbers are reused in multiple "Codes," so knowing "section 8001" doesn't tell you much.

Some laws are "laws," and some are "acts." There appears to be no difference. Section identifiers may end with letters, leading to the practice of writing "subdivision" between the cited section and the subsection, since 501b could be a law or it could be a subsection.

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
(((([A-Za-z\s]*)\sCode\s)([A-Za-z\s]*))?)(§|section|sections)(\s?)([0-9]{1})([0-9a-z\.]*)
```
