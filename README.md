# Node.js Manual & Documentation (.pdf, .mobi, .epub)

It all started with my desire to have a nicely formatted version of the node.js manual & documentation
as a printable pdf with a cover, table of content, indented code blocks and so on. Then came requests for a .mobi (Kindle)
file and an .epub (iOS, Android and more) file. --- Micro Zeiss (node 01.10.26)

I needed a pdf version of the current node.js manual, i searched on google, i couldn't find any, then i saw this project (that started 9 years ago- 2014). I refined it to my taste --- Elijah Echekwu (node 20.10.0)

### This is a my refinement to the project, originally started by Micro Zeiss
- [Github](https://github.com/zeMirco/nodejs-pdf-docs/)

Of course the whole creation and conversion process is written in node.js.

Current version of node.js in the docs: **20.10.0**

## How to use

Just check out the different folders or download directly:

- [pdf](https://github.com/Elijah57/node-js-manual/blob/main/pdf/nodejs-manual-1.pdf)
- [epub](https://github.com/Elijah57/node-js-manual/blob/main/epub/nodejs-manual.epub)


## Create your own files

You need to have [pandoc](http://johnmacfarlane.net/pandoc/) installed on your system. All the markdown files from the
[node repository](https://github.com/joyent/node) should be placed inside the markdown folder.

### Create .pdf

1. Use `node app.js` to create the .tex files
2. Manually edit the few files as shown in all.tex (or run `node cleanTex.js`)
3. Create the pdf with pdfLaTeX
4. (Optional) - use an online EPUB to PDF converter (Recommended)

#### Customizing

Use options.tex and run latex to customize your own manual.

### Create .epub

1. Run `node epub.js` to create the file

### Create .mobi

The .mobi version is created from the .epub file which gives better results compared to converting the .pdf file.

1. Download `kindlegen` from this repository or directly from [Amazon](http://www.amazon.com/gp/feature.html?ie=UTF8&docId=1000234621)
2. Run `node mobi.js` to create the file. The file is located inside the epub folder

## License

Copyright (C) 2023 [Elijah Echekwu](mailto: elijahechekwu30@gmail.com)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
