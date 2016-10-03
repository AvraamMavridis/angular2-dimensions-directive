# angular2-dimensions-directive
Fires an Event with the (initial) dimensions of a DOM element and also whenever the dimensions change

[![npm version](https://badge.fury.io/js/angular2-clickoutside-directive.svg)](https://badge.fury.io/js/angular2-clickoutside-directive)

[![forthebadge](http://forthebadge.com/images/badges/built-with-love.svg)](http://forthebadge.com)

## Install

`npm i angular2-dimensions-directive --save`

### Import the directive to your project and use it in your Component defining an event handler that is called whenever the dimensions of the element change

```typescript
import { DimensionsDirective } from 'angular2-clickoutside-directive';

@Component({
  selector: 'my-app',
  template : `
  <div clickOutside (onDimensionsChange)="onDimensionsChangeHandler($event)"">
    A button
  </button>`,
  directives : [  ClickOutsideDirective ]
} )
class MyFirstComponent implements OnInit {
  constructor(){}

  onDimensionsChange($event)
  {
    console.log( $event.dimensions )
  }

  ngOnInit(){}
}
```
### Contribute

Any pull-request is more than welcome :boom: :smile:

This project adheres to the Contributor Covenant [code of conduct](http://contributor-covenant.org/). By participating, you are expected to uphold this code.

### License

MIT
