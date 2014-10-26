# Ember-moment

[moment.js](momentjs.com) template helpers for ember [![Build Status](https://travis-ci.org/stefanpenner/ember-moment.svg?branch=master)](https://travis-ci.org/stefanpenner/ember-moment)

## Usage

* `npm install --save ember-moment`
* `ember g ember-moment`

```hbs
{{moment date}}
{{ago date}}
```

advance

```hbs
{{moment date inputFormat outputFormat}}
{{ago date inputFormat}}}
```

## Computed Macro

```js
import { moment, ago } from 'ember-moment/computed';

export default Ember.Controller.extend({
  date: new Date('2013-02-08T09:30:26'),
  shortDate: moment('date', 'MM/DD/YYYY')
  timeSince: ago('date', true)
});
```

## Development

* `git clone` this repository
* `npm install`
* `bower install`
* `ember server`
* Visit your app at http://localhost:4200.

## Running Tests

* `ember test`
* `ember test --server`

## Building

* `ember build`

For more information on using ember-cli, visit [http://www.ember-cli.com/](http://www.ember-cli.com/).
