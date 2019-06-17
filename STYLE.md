Headings
--------

Copy headings from the NIV, then:

- Ensure wording is consistent with body text (eg, NIV tends to use "festival" where KJV uses "feast").
- Ensure spelling is consistent with body text (eg, names may be transliterated differently).
- Avoid hyphenation and variable spacing (insert `\newline` for all breaks)


Body text
---------

Copy body text from the KJV, then:

- Use "God" instead of "GOD".
- Use smallcaps instead of block capitals.  Handy definitions are:
  - `\LORD`
  - `\LORDs`
- Use "Passover" instead of "passover".
- Use "Sabbath" instead of "sabbath".

Words consisting of block capitals can be found with `egrep`:

```bash
egrep '\b[A-Z][A-Z]+\b' filename.tex
```

Layout
------

Use `\columnbreak` and `\flushcolsend` where necessary, for example:

- A chapter starts too close to the bottom of a column (3 lines of text or fewer before the break)
- A heading is separated from the following content by a break

As a rule of thumb:

- At the bottom of a left-hand column, use `\vfill\columnbreak`
- At the bottom of a right-hand column, use `\flushcolsend\columnbreak`

...but see what works best.  Sometimes the extra spacing added by just
using a `\coolumnbreak` may be fine.

Comment all manual layout adjustments with `% layout hack` so they're easy to grep for.
