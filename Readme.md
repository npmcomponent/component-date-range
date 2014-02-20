*This repository is a mirror of the [component](http://component.io) module [component/date-range](http://github.com/component/date-range). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/component-date-range`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# date-range

  DateRange component

## Installation

    $ component install component/date-range

## Example

```js
var DateRange = require('./');

var now = new Date;
var future = new Date(Date.now() + 60000 * 5);
var range = new DateRange(now, future);
```

## API

### DateRange()

  Initialize a new DateRange `from` one date `to` another. If
  one date is larger than the other they are normalized so that `.from()`
  is always the smallest date.

### DateRange#from([date]:Date)

  Set / get from `date`.

### DateRange#to([date]:Date)

  Set / get to `date`.

### DateRange#diff()

  Return diff in milliseconds

### DateRange#toJSON()

  Return JSON representation.

### DateRange#equals(other:DateRange)

  Check if this range is identical to `other`.

### DateRange#toString()

  Return string representation.

## License

  MIT
