# Open Source Pentest Docs: Pitch

[![Build Status](https://travis-ci.org/OpenSourcePentest/pitch.svg?branch=master)](https://travis-ci.org/OpenSourcePentest/pitch)

The initial conversation slides and menu of scenarios

- Live Version: https://opensourcepentest.github.io/pitch/ (Automatically built and deployed on every commit)
- PDF-able Version: https://opensourcepentest.github.io/pitch/?print-pdf

## Reference Material: 

- https://room362.com/post/2017/open-source-pentesting/

This project uses [asciidocs]() through the backend called [asciidoctor-reveal](https://github.com/asciidoctor/asciidoctor-reveal.js/).

If you need help with AsciiDoc syntac refer to their user guide here: http://www.methods.co.nz/asciidoc/userguide.html

## Requirements to build

```
mubix@host:~$ gem install 'asciidoctor-revealjs'
```

## Building

1. Close the respository
```
mubix@host:~$ git clone https://github.com/OpenSourcePentest/pitch
```

2. Change directory into the `pitch` directory and pull down Reveal.js into the `revealjs` directory

```
mubix@host:~$ cd pitch
mubix@host:~/pitch/$ git clone -b 3.5.0 --depth 1 https://github.com/hakimel/reveal.js.git revealjs
```

3. Build the `index.html`

```
mubix@host:~/pitch/$ asciidoctor-revealjs -o index.html index.adoc
```

Thats it.. 

.. or you can cheat and just check out the version that Travis builds on very commit:

```
git clone -b gh-pages https://github.com/OpenSourcePentest/pitch.git
```
