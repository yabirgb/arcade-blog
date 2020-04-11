Title: Arcade: A new static site generator
Date: 07-04-2020
Author: Yábir García
Tags: ['projects']

I want to make a little post talking about `Arcade`, my latest public
project. 

The objetive was to create an easy to use static site generator that
didn't require a complex installation process and let me quicly focus
on just writting. Previously my blog was generated using hugo, but my
biggest issue was that I needed to have go and install the
dependencies. Whenever I wanted to write something it just happend
that I didn't have the right tools installed and I had to go to the
documentation and restart the installation process. Also `go` doesn't
come by default in my system, so I have to worry about having it
installed.

For this reasons I wanted to create something that was just `plug and
write` and allowed me as much as hugo did.

## The tooling

I went with python3 because most of the linux distros (if not all of
them) bring python by default in the system and to install my package
you only need pip and an easy

```python3 -m pip install arcade-generator```

and you have everything you need.

## Capabilities 

I did't want to lose some good things from hugo like:

- command line utility
- live server that shows changes after saves
- easy script to create the basic folder structure
- theme system

those are strong points that I believe every static site generator
should have and arcade must match those.

## How I did it

It surprised me because it was quite easy. In one afternoon I had more
or less the basic code without much effort.

To read commands from the command line I used
[click](https://click.palletsprojects.com/en/7.x/) wich I've used
previously and makes everything related to command line tools
consistant, conviniant and easy.

To get live previous of my files I used
[livereload](https://github.com/lepture/python-livereload). Again
super easy to use and provided much all the features I was looking
for.

To get my markdown text to html I use the
[markdown](https://python-markdown.github.io/) package. It supports
many of the things you can imagine from markdown so it was the obvious
decission.

On my side what I did was to track for changes the `content` and
`themes` folder so every time something changes on disk the html files
are updated. I provided basic functionalities like a `most recent`
section, `history` of posts and configurable social icons.

Finally to make easy to use themes I use `jinja` so everything is
passed to certain variables and the only thing left to do if you want
a new theme is edit the templates.

There are 3 basic commands

- `init`
- `watch`
- `build`

The last one builds all the html structure with the static content and
prepares it in a folder ready to be uploaded.

## The future

In the future I want to add more functionalities like integration with
`github-packages` and optimizations in the source code. 

Hope you enjoy it!
