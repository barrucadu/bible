The King James Bible
====================

![In the beginning God created the heaven and the earth](preview.png?raw=true)

I am using LaTeX to typeset the King James Bible.

You can see the latest version here: https://misc.barrucadu.co.uk/artefacts/bible/master.pdf


Building
--------

You will need XeLaTeX and the (non-free) [Equity][] font to compile
this.  If you don't have Equity, you could substitute in another font
but it won't look the same as my version (obviously).

```bash
$ latexmk -xelatex main.tex
```

The font declarations in `main.tex` assume the Equity files are in
`~/s/fonts/equity`.

[Equity]: https://typographyforlawyers.com/equity.html

Q & A
-----

**Why are you doing this?**

I realised that I'd used LaTeX a lot (eg, for my Ph.D thesis), but I'd
never really tried making something with the primary purpose being to
look good.

So this project is an opportunity for me to learn how to do that sort
of thing.

**Why the Bible?  Are you religious?**

No.  It was this or poetry, and I couldn't pick a poem.

**Why the *King James* Bible?**

1. It's in the public domain, which more recent translations might not
   be.

2. I feel like fancy typesetting and fancy language go well together.
