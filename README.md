# It's the Phoenix Spokes People website.

## Summary

It's built with [GitHub Pages](https://pages.github.com/) and [Jekyll](https://jekyllrb.com/).

You'll probably want to be a bit familiar with git first, because that's how you make changes. [Here is a fun tutorial](https://try.github.io/levels/1/challenges/1).


## Development

1. Open in devcontainer
1. Wait a bit
1. `$ jekyll watch`
1. Wait a bit
1. Open http://127.0.0.1:4000/

## Components

### Static pages

* [Home page](https://github.com/phoenixspokespeople/phoenixspokespeople.github.io/blob/master/index.md)
* [About](https://github.com/phoenixspokespeople/phoenixspokespeople.github.io/blob/master/about.md)
* [Contact](https://github.com/phoenixspokespeople/phoenixspokespeople.github.io/blob/master/contact.md)
* [Hello page](https://github.com/phoenixspokespeople/phoenixspokespeople.github.io/blob/master/hello.md)

### Dynamic pages

The [events page](https://github.com/phoenixspokespeople/phoenixspokespeople.github.io/blob/master/events/index.html) is clever.
It is populated from all the events in the [events collection](https://github.com/phoenixspokespeople/phoenixspokespeople.github.io/tree/master/_events).

Because it's a static site I just use the `published` flag to hide events in the past. It's not great, but it works.

### Images

Go in the [images folder](https://github.com/phoenixspokespeople/phoenixspokespeople.github.io/tree/master/images).
