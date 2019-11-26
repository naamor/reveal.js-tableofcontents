# reveal.js-tableofcontents

A table of contents plugin for [Reveal.js](https://github.com/hakimel/reveal.js) to generate automatically a table of contents slide. [Check out the live demo](https://naamor.github.io/reveal.js-tableofcontents/).

## Installation

### npm

Download and install the package in your project:

```npm install --save reveal.js-tableofcontents```

Add the plugin to the dependencies in your presentation:

```javascript
Reveal.initialize({
    // ...

    dependencies: [
        // ...

        { src: 'node_modules/reveal.js-tableofcontents/tableofcontents.js' }
    ]
});
```

### Manual

Copy this repository into the plugins folder of your reveal.js presentation, i.e. ```plugins/tableofcontents```.

Add the plugin to the dependencies in your presentation:

```javascript
Reveal.initialize({
    // ...

    dependencies: [
        // ...

        { src: 'plugin/tableofcontents/tableofcontents.js' }
    ]
});
```

## Configuration

You can configure the table of contents for your presentation by providing a ```tableofcontents``` option in the reveal.js initialization options. Note that all configuration values are optional and will default to the values specified below.

```javascript
Reveal.initialize({
    // ...

    tableofcontents: {
        // Specifies the slide title of the table of contents slide
        title: "Table of Contents",

        // Specifies the position of the table of contents slide in the presentation
        position: 2,

        // Specifies html tag in which the table of contents title stands
        titleTag: "h1",

        // Specifies which slide tag elements will be used
        // for generating the table of contents.
        titleTagSelector: "h1, h2, h3, h4, h5, h6",

        // Specifies if the first slide, mostly the title slide of the presentation, should be ignored.
        ignoreFirstSlide: false,

        // Specifies if every single element of the table of contents
        // will be stepped through before moving on to the next slide.
        fadeInElements: false
    },
});
```

## License

[MIT licensed](https://en.wikipedia.org/wiki/MIT_License)

Copyright (C) 2018 Roman Stocker
