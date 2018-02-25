<ul>
  <li><a href="#marked">About</a></li>
  <li><a href="#install">Installation</a></li>
  <li><a href="#usage">Usage</a></li>
  <li><a href="#specifications">Supported Markdown specifications</a></li>
  <li><a href="#contributing">Contributing</a></li>
  <li><a href="#authors">Authors</a></li>
  <li><a href="#license">License</a></li>
</ul>

<h2 id="marked">About</h2>

Marked is 

1. built for speed.<sup>*</sup>
2. a low-level markdown compiler that allows frequent parsing of large chunks of markdown without caching or blocking for long periods of time.<sup>**</sup>
3. light-weight while implementing all markdown features from the supported flavors & specifications.<sup>***</sup>
4. available as a command line interface (CLI) and running in client- or server-side JavaScript projects.

<p><small><sup>*</sup> Still working on metrics for comparative analysis and definition.</small><br>
<small><sup>**</sup> As few dependencies as possible.</small><br>
<small><sup>***</sup> Strict compliance could result in slower processing when running comparative benchmarking.</small></p>

<h2 id="installation">Installation</h2>

**CLI:** `npm install -g marked`

**In-browser:** `npm install marked --save`

<h2 id="usage">Usage</h2>

**CLI**

``` bash
$ marked -o hello.html
hello world
^D
$ cat hello.html
<p>hello world</p>
```

**Browser**

```html
<!doctype html>
<html>
<head>
  <meta charset="utf-8"/>
  <title>Marked in the browser</title>
  <script src="/path/to/marked.min.js"></script>
</head>
<body>
  <div id="content"></div>
  <script>
    document.getElementById('content').innerHTML =
      marked('# Marked in browser\n\nRendered by **marked**.');
  </script>
</body>
</html>
```


Marked offers [advanced configurations](https://github.com/markedjs/marked/blob/master/USAGE_ADVANCED.md) and [extensibility](https://github.com/markedjs/marked/blob/master/USAGE_EXTENSIBILITY.md) as well.

<h2 id="specifications">Supported Markdown specifications</h2>

We actively support the features of the following [Markdown flavors](https://github.com/commonmark/CommonMark/wiki/Markdown-Flavors).

|Flavor                                                     |Version    |
|:----------------------------------------------------------|:----------|
|The original markdown.pl                                   |--         |
|[CommonMark](http://spec.commonmark.org/0.28/)             |0.28       |
|[GitHub Flavored Markdown](https://github.github.com/gfm/) |0.28       |

By supporting the above Markdown flavors, it's possible that Marked can help you use other flavors as well; however, these are not actively supported by the community.


<h2 id="contributing">Contributing</h2>

The marked community enjoys a spirit of collaboration and contribution from all comers. Whether you're just getting started with Markdown, JavaScript, and Marked or you're a veteran with it all figured out, we're here to help you improve as a professionally while helping improve Marked technically. Please see our [contributing documentation](https://github.com/markedjs/marked/blob/master/CONTRIBUTING.md) for more details.

For our Contribution License Agreement, see our [license](https://github.com/markedjs/marked/blob/master/LICENSE.md).

<h2 id="authors">Authors</h2>

For list of credited authors and contributors, please see our [authors page](https://github.com/markedjs/marked/blob/master/AUTHORS.md).

<h2 id="license">License</h2>

Copyright (c) 2011-2018, Christopher Jeffrey. (MIT License)

See [license](https://github.com/markedjs/marked/blob/master/LICENSE.md) for more details.

