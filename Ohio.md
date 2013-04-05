Example section numbers:

* 105.25
* 3111.211

Cross-references:

* sections 3111.01 to 3111.18 or 3111.20 to 3111.85 
* section 3111.211 or 5101.314 or section 2151.232 of the Revised Code

Cross-references are prefixed with "section," rather than "§".

The simplicity of Ohio's citations are tricky. They don't reliably use the word "section" beforehand, they never use the section symbol (§), and so all that we're left with is a string of 5–7 numbers, separated by a single hyphen.

The titles are 1–2 digits. Chapters are 3–4 digits, with the first 1–2 digits consisting of the title number. And sections are the chapter number, a decimal, and then a 2–3 digit number. Section numbering generally begins at ".01" and increments sequentially.

Here's a regular expression that works for vanilla uses and for cross-references:

```
([0-9]{3,4})\.([0-9]{2,3})
```

There will be some over-broad matches, but there's no getting around it.

They sort with proper decimal sorting, rather than as if the decimals were whole numbers. For example, see [the order of Chapter 5727](http://codes.ohio.gov/orc/5727): they use proper decimal sorting—.10, .11, .111, .12.
