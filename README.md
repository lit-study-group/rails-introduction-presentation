# rails-introduction-presentation

## How to run

```
npm install -g grunt-cli bower yo generator-reveal
npm install
bower install
grunt server
```

## Creating new slides

To create a new slide, run the command

```
yo reveal:slide "SLIDENAME" --markdown
```

SLIDENAME will be the file name so it should be ASCII characters.

You then just have to write the slide created at slides/SLIDENAME.md

## Documentation:

* [RevealJS](https://github.com/hakimel/reveal.js)
* [Yo reveal](https://github.com/slara/generator-reveal)
