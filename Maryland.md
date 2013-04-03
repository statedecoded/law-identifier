Example section numbers:

* § 10A-101
* § 5-7B-08
* § 14-1012
* § 14-102.1

As used within citations within the code:

* under § 2-205, § 4-205, or § 6-202 of this article
* § 3-307 of the Criminal Law Article
* § 5-202 of this subtitle
* § 9-301 of the State Government Article
* § 5-7B-03 of this subtitle
* §§ 13-1101 and 13-1111 of the Financial Institutions Article
* § 19-115 of this title

As used within court decisions:

* Section 10-222(c) of the State Government Article of the Maryland Code
* Section 32(h)
* Section 22(a)(9) of Article 49B of the Maryland Annotated Code
* Code, Courts Article, § 12-603
* Section 12-603 of the Courts and Judicial Proceedings Article, Maryland Code

There's a citation translation guide in Md. Ann. Code art. 1, § 25. (I'd provide a link, but the Maryland Code is only available via LexisNexis' site, which has unlinkable, stateful URLs.) Here's a snippet:

> (b) Agriculture Article. -- A section of the Agriculture Article may be cited as: "§      of the Agriculture Article".
> 
> (c) Business Occupations and Professions Article. -- A section of the Business Occupations and Professions Article may be cited as: "§      of the Business Occupations and Professions Article".
> 
> (d) Business Regulation Article. -- A section of the Business Regulation Article may be cited as: "§      of the Business Regulation Article".
> 
> (e) Commercial Law Article. -- A section of the Commercial Law Article may be cited as: "§      of the Commercial Law Article".

That provides a lookup table.

Here's a pretty good PCRE:

```
(((§|Section)\s)?)([0-9]+)([a-zA-Z]?)-([0-9]+)([a-zA-Z]?)((-?)([0-9]+)([a-zA-Z0-9\.]*)?)((\sof th(e|is) ([A-Za-z ]+))?)
```

It fails to capture:

* Section 32(h)
* Section 22(a)(9) of Article 49B of the Maryland Annotated Code
* Section 22(a)(9) of Article 49B of the Maryland Annotated Code

And it only captures the final portion (§ 12-603) of:

* Code, Courts Article, § 12-603
* 
