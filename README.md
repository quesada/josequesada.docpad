josequesada.docpad
==================
I'm a data scientist. This is the 4th reincarnation of my website. Learning proper js/coffescript is one of my goals, because node's stream-based worldview looks like could be important for analytics-in-motion (vs analytics-at-rest).

This site is done with Docpad, which uses node.js.

Docpad gets lots of updates, and so do the plugins. It's easier to update them all (and docpad), by issuing:

    $ npm update

Note the lack of sudo, and npm -g. The [install instructions](http://bevry.me/learn/docpad-install) recommend to install docpad globally, but this way it's easier to be up-to-date:

    $ ln -s node_modules/docpad/bin/docpad .

Then, use it as:
    
    $ ./docpad 

About the node ecosystem... 

1- The package manager kicks ass. if you are used to rvm or virtualenv+pip, the node way of this is refreshing:

- Everything install locally by default (built-in virtualenv)
- Semantic versioning (ie, specify what version of a plugin you need)
- Each package can have isolated dependencies. That is, two packages might be using different versions of a package as a dependency

2- The [node aesthetic](http://substack.net/posts/b96642) goes a long way to promote radical reusability. This is very similar to the unix philosophy (do one thing only, and do it well). Packages are tiny, when you install one it looks like it's downloading half the internet: reusability is very high. 

For these two reasons, node's community moves at blazing speeds.

Thanks to:

- Ben Lupton for [docpad](http://docpad.org). He's very commited to making docpad the best CMS possible. Still too geeky for the masses, but in the future docpad could dethrone wordpress.
- [Ben Delarre](http://www.delarre.net/) for his pagination plugin and sharing the code for his bootstrap-basd docpad blog.
- 
