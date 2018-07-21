# single-result

A Polymer Element showing a single stylized result with images, extractions, details, and other optional information.

### Example
```js
demo.headerExtractions = [{
  name: 'Built By',
  data: [{
    confidence: 'high',
    highlight: true,
    icon: 'star',
    link: 'https://nextcentury.com',
    text: 'Next Century'
  }]
}];

demo.details = [{
  name: 'Description',
  text: 'DigElements is a library of common Polymer Elements built by Next Century Corporation.'
}];

demo.detailExtractions = [{
  name: 'My Favorite DigElements',
  data: [{
    confidence: 'high',
    highlight: true,
    icon: 'link',
    link: 'https://github.com/usc-isi-digelements/single-result',
    text: 'Single Result'
  }]
}];

demo.images = [{
  link: 'https://github.com/DigElements',
  source: 'dig.png'
}];
```

```html
<single-result
  flag="Important"
  highlighted-text="The <em>DigElements</em> library."
  icon="favorite"
  link="https://github.com/DigElements"
  rank="0.99"
  type="Webpage"
  headerExtractions="[[headerExtractions]]"
  details="[[details]]"
  detailExtractions="[[detailExtractions]]"
  images="[[images]]">
</single-result>
```

### Dependencies

Dependencies are installed using [Bower](http://bower.io/):

    npm install -g bower
    bower install

### Testing

Tests are run using [web-component-tester](https://github.com/Polymer/web-component-tester):

    npm install -g web-component-tester
    wct

### Demonstration & Documentation

Demonstration and documentation are viewed using [polyserve](https://github.com/PolymerLabs/polyserve):

    npm install -g polyserve
    polyserve

