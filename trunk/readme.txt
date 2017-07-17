=== Pygment It ===
Contributors: glauco_dsc
Donate link: https://pledgie.com/campaigns/26327
Tags: syntax, highlighter, pygment, highlighting
Requires at least: 3.0.1
Tested up to: 3.4
Stable tag: 1.0
License: MIT
License URI: http://opensource.org/licenses/MIT

A WordPress plugin for syntax highlighting using Pygments, though Pygments is not required to be installed.

== Description ==

By default, Pygment It will auto discover if Pygments is installed (through command -v pygmentize). If not, it will use http://pygments.appspot.com to highlight code (but without support for: highlighted lines, line numbers and line number to start).

* Syntax-highlighted code cached as post metadata
* Admin panel to choose theme, default language and Pygments usage (local, external API or auto discover)
* Multiple themes available (github, monokai, railscasts, mustang, among others..)
* Support for `hl_lines` (highlighted lines), `linenos` (line numbers) and `linenostart` (line number to start) when using a local installation of Pygments
* Works with all Pygments's supported languages (the full list can be found <a href="http://pygments.org/languages/" target="_blank">here</a>)

#### Usage

Using default language set in admin:
```
[code]
  # code here
[/code]
```

Choosing language:
```
[code language="ruby"]
  # Ruby language syntax highlighting
[/code]
```

Highlighting lines 2 and 3:
```
[code language="ruby" hl_lines="2 3"]
  class PagesController < ApplicationController
    def index
    end      
  end
[/code]
```

Displaying lines, starting with 20:
```
[code linenos="table" linenostart="20"]
  # code here
[/code]
```

#### Contributing

Send your contribution for <a href="https://github.com/glaucocustodio/pygment-it" target="_blank">this github repo</a>.

== Installation ==

This section describes how to install the plugin and get it working.

1. Upload plugin's content to `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress

== Frequently Asked Questions ==

= Must I have Pygments installed in my server? =

No, in case your server does not have Pygments installed, the plugin will use an external api to perform syntax highlight

== Screenshots ==

1. screenshot-1.png 
2. screenshot-2.png

== Changelog ==

= 1.0 =
* Plugin creation

== Upgrade Notice ==

= 1.0 =
Plugin creation
