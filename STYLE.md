Headings
--------

Copy headings from the NIV, then:

- Ensure wording is consistent with body text (eg, NIV tends to use "festival" where KJV uses "feast").
- Ensure spelling is consistent with body text (eg, names may be transliterated differently).


Body text
---------

Copy body text from the KJV, then:

- Use "God" instead of "GOD".
- Use smallcaps instead of block capitals.  Handy definitions are:
  - `\LORD`
  - `\LORDs`
- Use "Passover" instead of "passover".

Words consisting of block capitals can be found with `egrep`:

```bash
egrep '\b[A-Z][A-Z]+\b' filename.tex
```

Layout
------

Use `\columnbreak` and `\flushcolsend` where necessary.
