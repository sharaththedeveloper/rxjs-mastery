# Of

> Create an observable

``` javascript
import { of } from 'rxjs';

const obs$ = of('first value','second value');
obs$.subscribe(data=>console.log(data))

// emits values
/*
	first value
	second value
*/
```

