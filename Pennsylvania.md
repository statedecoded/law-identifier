Examples within the code:

* § 149.9
* § 138k.13
* § 59.4a
* Rule 1205

Section identifiers are are the chapter number, a period, and then a unique identifier within that chapter. They are often (but not always) preceded by a §. Except when they’re “rules,” and then they’re simply an incremented number (with the first two characters representing the chapter number). Rules are found within titles with “rules” in their name (e.g., “Rules of Evidence,” “Minor Court Civil Rules”).

Section identifiers are not unique within the code, only within the title.

From court rulings:

* Section 9543.1 of the Post Conviction Relief Act (“PCRA”), 42 Pa.C.S.A. § 9543.1
* 42 Pa.C.S. § 702(b)
* 18 Pa.C.S.A. § 907(a)
* Section 314(a) of the Workers’ Compensation Act (“Act”), 77 P.S. § 651(a)
* Section 704 of the Administrative Agency Law, 2 Pa.C.S. § 704
* 1 Pa.C.S. § 1921(a)

Subsequent references begin with “id. "

Here's a fairly good regex:

```
((\d{1,2}\sPa?\.(C\.)?S\.(A\.)?\s)?(§|Rule|Section)\s?\d{1,4}\(?[a-z]?\)?(\.\d{1,3}[a-z]?)?(\sof\sthe\s[A-Za-z “”’()]+)?(, )?){1,2}
```
