# Angular2 - Displaying Data

## Pre-requirement
```
$ npm install -g tsd
$ npm install -g typescript@^1.5.0-beta
```

## Run the TypeScript compiler
```
$ tsd query angular2 --action install
$ tsc --watch -m commonjs -t es5 --emitDecoratorMetadata {$typescript}
```

## Import Angular
Inside of typescript, import the type definitions from Angular:
```typescript
/// <reference path="typings/angular2/angular2.d.ts" />
```
The editor should be able to complete the available imports:
```typescript
import {Component, View, bootstrap} from 'angular2/angular2';
```
### Overall structure
```typescript
/// <reference path="typings/angular2/angular2.d.ts" />
import {Component, View, bootstrap} from 'angular2/angular2';

@Component({
  ...
})

@View({
  ...
})

class DisplayComponent {
  ...
}

bootstrap(DisplayComponent);
```

Reference: [5 MIN QUICKSTART](https://angular.io/docs/js/latest/quickstart.html)