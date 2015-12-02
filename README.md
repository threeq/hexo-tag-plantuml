## Introduction

This is a [hexo](https://github.com/tommy351/hexo)
tag plugin which allows you to render plantuml code in you blog.

Hexo is a static blogging system written in Node.js.
But hexo no support plantuml tag

## Installation

To install, run the following command in the root directory of hexo:
```
npm install hexo-tag-plantuml --save
```

And add this plugin in your ``_config.yml``.

## Usage

_config.yml add config:

	tag_plantuml:
		type: static

**static**: download svg image into html file, "data:image/svg+xml;utf8";
**dynamic**: use http://www.plantuml.com/plantuml/svg dynamic produce

Specify the code filetype, and whether to use line number in your markdown source file, in the common format of tag plugins:

	{% plantuml %}
        Bob->Alice : hello
	{% endplantuml %}

