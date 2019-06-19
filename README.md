# QML (Quantum Markup Language)

![Draft](https://img.shields.io/badge/Draft-In%20progress-yellow.svg) ![Not implemented](https://img.shields.io/badge/Status-Not%20implemented-red.svg)

Smaller and faster than JSON and HTML.
QML is based on Emmet as HTML is based on XML; with improvements (such as support to datasets) and Esperanto as main language.

- Lightweighter as possible
- Hightly semantic
- Context-aware

## Comparison

### vs. HTML

HTML:

```
<body id="korp"><header id="kaplok"></header><content id="enhavo"><article id="artikol" class="blog">Article`s content</article></content></body>
```

QML:

```
korp#body>kaplok.header+enhavo#content>artikol#article.blog{Article`s content}
```

While JSON is sometimes faster to parse than HTML, it gives more bytes to read/download.
But QML language is faster than both JSON and HTML, and also uses less bytes.
HTML uses 70-75 more characters than QML.

QML is also smaller as well when visualy (human-readable) structured, compared to HTML:

```
korp#body>
	kaplok.header+
	enhavo#content>
		artikol#article.blog{Article`s content}
```

```
<body id="korp">
	<header id="kaplok"></header>
	<content id="enhavo">
		<article id="artikol" class="blog">Article`s content
		</article>
	</content>
</body>
```

HTML uses 3 more lines than QML.

### vs. JSON

QML as a data store:
		
```
users>
	alice>
		fulln=Alice Althea+
		addr=dataddress^
	bob>
		fulln=Bob Bulbasaur+
		addr=dataddress
```

Compared to JSON:

```
{
"users":[{
"alice":[{
"fulln":"Alice Althea",
"addr":"dataddress"
}],
"bob":[{
"fulln":"Bob Bulbasaur",
"addr":"dataddress"
}]
}]
}
```

Single-line JSON datastore:

```
{"users":[{"alice":[{"fulln":"Alice Althea","addr":"dataddress"}],"bob":[{"fulln":"Bob Bulbasaur","addr":"dataddress"}]}]}
```

Single-line QML datastore:

```
users>alice>fulln=Alice Althea+addr=dataddress^bob>fulln=Bob Bulbasaur+addr=dataddress
```

QML haves 5 lines & 32-41 characters less than JSON.

### vs. Emmet

- QML haves Esperanto as main language, while Emmet uses English
- QML is also used for datastores
- QML supports human-readable, word-wrapped identation

## Contributing

This is a open-source and accessible markup language, so you're welcome to open a issue (with criticism/suggestions) and open pull requests with improvements.
Please follow our <a href="http://www.contributor-covenant.org/" target="_blank">Code of Conduct</a> before interacting or contributing.

## Todo

- Site
- Profile+Blog
- Manifesto
- License
- Script that is firstly downloaded, and works offline for rendering QML into HTML on classic browsers
- JML.js
- .qml
- .qmlx (16-bit compressed, prioritized from slow online conn)
- Works on Kaypi
- Render markdown for faster parsing (use MD instead of own tags)
- Embed, sandbox QML (a social network can enable posting in QML)
- Op Gv
- https://en.wikipedia.org/wiki/Semantic_Web#Limitations_of_HTML

## Related links

<a href="https://emmet.io/" target="_blank">Emmet Markup Language</a> (in which QML is based)