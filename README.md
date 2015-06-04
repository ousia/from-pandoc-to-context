# pandoc-xhtml

`pandoc-xhtml.tex` offers a way to compile _Markdown_ documents with ConTeXt.

`pandoc-xhtml.tex` is an environment, which is what ConTeXt needs to compile XML sources directly.

With the proper environment, ConTeXt deals with XML natively. It doesn’t need any intermediate format. Not even a ConTeXt source file cotaining the text to be typeset.

## What Is Wrong with ConTeXt Sources?

`pandoc` can generate ConTeXt documents from _Markdown_ sources. But this way you’ll miss:

* Main document language information.

* Markup for language in text portions.

* Any `<div>` or `<span>` elements markup.

Generating the PDF document from XML sources with ConTeXt avoids loosing relevant information (such as language, which result in wrong hyphenation) or special layout for block or inline elements.

Going this way, the _Mardown_ source document may fullfill the promise:

> One source to generate them all.

## Status

This project is still work in progress. I have used myself to publish a book and some other documents. It fits my needs.

Of course, my documents may contain code, but no math. My texts contain some expressions in foreign languages and some code.

The documentation needs some polishing to be released. I hope to have it finished by the end of June 2015.

If you find something that can be improved or you want to comment anything related to the project, please [open an issue](https://github.com/ousia/from-pandoc-to-context/issues/new).

## License

The environment file from this project (`pandoc-xhtml.tex`) is licensed to the public under the GNU General Public License; either [version 2](https://www.gnu.org/licenses/gpl-2.0.html), or (at your option) any [later version](https://www.gnu.org/licenses/gpl.html).

The documentation is released under the [_Creative Commons_ Attribution–ShareAlike 4.0 International license](https://creativecommons.org/licenses/by-sa/4.0/).

## Acknowledgments

This work was based on the extraordinary achievements of John MacFarlane and Hans Hagen.

I want to thank them for their software and their help.
