# Finnish and Swedish (`apertium-fin-swe`)

This is an Apertium language pair for translating between *Finnish* and
*Swedish*. What you can use this language package for:

* Translating between Finnish and Swedish
* Morphological analysis of Finnish and Swedish
* Part-of-speech tagging of Finnish and Swedish

For information on the latter two points, see subheading [For more
information](#For-more-information) below.

## Requirements

You will need the following software installed:

* lttoolbox (>= 3.3.0)
* apertium (>= 3.3.0)
* vislcg3 (>= 0.9.9.10297)
* hfst (>= 3.8.2)
* apertium-fin
* apertium-swe

If this does not make any sense, we recommend you look at: www.apertium.org

## Compiling

If the requirements are installed, you should be able to just run:

```
$ ./configure
$ make
# make install
```

After the first checkout you may need to run `./autogen.sh`.

## Testing

If you are in the source directory after running make, the following
commands should work:

```
$  echo "talo" | apertium -d . fin-swe
hus
$ echo "ett hus" | apertium -d . swe-fin
yksi talo
```

## Files and data

* `apertium-fin-swe.fin-swe.dix`  - Bilingual dictionary
* `apertium-fin-swe.fin-swe.t1x`  - Chunking rules for translating into Swedish
* `apertium-fin-swe.swe-fin.t1x`  - Chunking rules for translating into Finnish
* `apertium-fin-swe.fin-swe.t2x`  - Interchunk rules for translating into Swedish
* `apertium-fin-swe.swe-fin.t2x`  - Interchunk rules for translating into Finnish
* `apertium-fin-swe.fin-swe.t3x`  - Postchunk rules for translating into Swedish
* `apertium-fin-swe.swe-fin.t3x`  - Postchunk rules for translating into Finnish
* `apertium-fin-swe.fin-swe.lrx`  - Lexical selection rules for translating into Swedish
* `apertium-fin-swe.swe-fin.lrx`  - Lexical selection rules for translating into Finnish
* `modes.xml`                     - Translation modes

## For more information

* http://wiki.apertium.org/wiki/Installation
* http://wiki.apertium.org/wiki/apertium-fin-swe
* http://wiki.apertium.org/wiki/Using_an_lttoolbox_dictionary

## Help and support

If you need help using this language pair or data, you can contact:

* Mailing list: apertium-stuff@lists.sourceforge.net
* IRC: `#apertium` on `irc.freenode.net`

See also the file AUTHORS included in this distribution.

