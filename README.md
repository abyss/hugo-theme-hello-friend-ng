# Hello Abyss

## General information

This theme is a modified version of [hello-friend-ng](https://github.com/rhazdon/hugo-theme-hello-friend-ng) by Djordje Atlialp. Check it out, maybe it will work better for your purposes. If you really like this theme, buy him a coffee.

You can see an example of this theme in use at https://abyss.dev.

---
## Features

- Dark Mode / Light mode, depending on your preferences (Default is Dark)
- Great reading experience thanks to [**Inter UI font**](https://rsms.me/inter/), made by [Rasmus Andersson](https://rsms.me/about/)
- Nice code highlighting thanks to [**PrismJS**](https://prismjs.com)
- An easy way to modify the theme with Hugo tooling
- Fully responsive
- Support for social icons
- Support for sharing buttons

### What hello-abyss changes over hello-friend-ng
- Posts use Date instead of Datetime
- Footer is more adjustable
- Hugo Environments can add additional menu or social menus via "extra"
- CanonicalURL can be overridden to a different domain
- Logo text is dynamic and changes per page
- Minor cosmetic changes
- Maybe other changes undocumented (sorry!)

## How to start

You can download the theme manually by going to [https://github.com/abyss/hugo-theme-hello-abyss](https://github.com/abyss/hugo-theme-hello-abyss) and pasting it to `themes/hello-abyss` in your root directory.

You can also clone it directly to your Hugo folder:

``` bash
$ git clone https://github.com/abyss/hugo-theme-hello-abyss themes/hello-abyss
```

You can also include it as a git submodule:

``` bash
$ git submodule add https://github.com/abyss/hugo-theme-hello-abyss themes/hello-abyss
```

## How to configure

Most of the configuration is the same as the original theme, however there are some customizations. If you are interested in using this theme, it may be helpful to see a live configuration at https://github.com/abyss/abyss.dev.

## More things

### Built-in shortcodes

There is one additional shortcode, created by Djordje.

#### image

Properties:

  - `src` (required)
  - `alt` (optional)
  - `position` (optional, default: `left`, options: [`left`, `center`, `right`])
  - `style`

Example:

``` golang
{{< image src="/img/hello.png" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}
```

### Code highlighting

Supported languages: [Take a look here](https://prismjs.com/download.html#themes=prism-tomorrow&languages=markup+css+clike+javascript+abap+actionscript+ada+apacheconf+apl+applescript+c+arff+asciidoc+asm6502+csharp+autohotkey+autoit+bash+basic+batch+bison+brainfuck+bro+cpp+aspnet+arduino+cil+coffeescript+clojure+ruby+csp+css-extras+d+dart+diff+markup-templating+docker+eiffel+elixir+elm+lua+erb+erlang+fsharp+flow+fortran+gcode+gedcom+gherkin+git+glsl+gml+go+graphql+groovy+less+handlebars+haskell+haxe+hcl+http+hpkp+hsts+ichigojam+icon+inform7+ini+io+j+java+scala+php+javastacktrace+jolie+n4js+markdown+json+julia+keyman+kotlin+latex+crystal+scheme+liquid+lisp+livescript+lolcode+makefile+django+matlab+mel+mizar+monkey+n1ql+typescript+nand2tetris-hdl+nasm+nginx+nim+nix+nsis+objectivec+ocaml+opencl+oz+parigp+parser+pascal+perl+php-extras+sql+powershell+processing+prolog+properties+protobuf+scss+puppet+pure+python+q+qore+r+jsx+renpy+reason+vala+rest+rip+roboconf+textile+rust+plsql+sass+stylus+smalltalk+smarty+soy+sas+twig+swift+yaml+tcl+haml+toml+tt2+pug+tsx+visual-basic+vbnet+velocity+verilog+vhdl+vim+wasm+wiki+xeora+xojo+xquery+tap)

By default the theme is using PrismJS to color your code syntax. All you need to do is to wrap you code like this:

<pre>
``` html
  // your code here
```
</pre>

## Known issues

There is a bug in Hugo that sometimes causes the main page not to render correctly. The reason is an empty taxonomy part.
Related issue tickets on hello-friend-ng repo: [!14](https://github.com/rhazdon/hugo-theme-hello-friend-ng/issues/14) [!59](https://github.com/rhazdon/hugo-theme-hello-friend-ng/issues/59).

Either you comment it out completely or you write the following in

``` toml
[taxonomies]
  tag      = "tags"
  category = "categories"
```

## Licence

The theme is released under the MIT License. Check [LICENSE.md](https://github.com/abyss/hugo-theme-hello-abyss/blob/master/LICENSE.md) for additional licensing information.
