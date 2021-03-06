# How to contribute

## Installation & compilation
Our documentation is made using Jekyll (http://jekyllrb.com/)

In order to contribute please install the following :

Run Jekyll server (on port 4000)
Inside your directory (ex: ~/dev/thelia.github.io/)

    $ jekyll serve --watch

To see the result : http://localhost:4000

In order to let the documentation be aware of your new page please fill in the file

    _config.yml

And reload Jekyll server

In addition, this documentation layout use [Bootstrap](http://getbootstrap.com) and this LESS files for CSS.

## Translations
A single directory represents one language. By convention, the name of the directory must correspond to [ISO 639-1 code](http://en.wikipedia.org/wiki/List_of_ISO_639-1_codes).

For each language, you must define : __name__ (English), __code__ (en), __url__ (/en) and __sidebar__.
To define this elements, you must edit the __\_config.yml__ file to add your language configuration like this :

```yml
languages:
  - {
      name: "English", code: "en", url: "/", sidebar:
      ...
    }
  - {
      name: "Your language", code: "ISO 639-1 code", url: "/url-to-language", sidebar:
      ...
    }
```
__The best way is to duplicate English configuration which is the most advanced.__ So you can duplicate english directory (en) and rename it with the correct language code.

After updated the __\_config.yml__ file, you have to restart your Jekyll server.

# Credits

Bootstrap is under MIT licence.