# First

> used to filter the first emitted value from the observable

``` javascript
import { of } from "rxjs";
import { first } from "rxjs/operators";
const obs1$ = of(1,2,3,4,5,6,7,8,9,10);
const obs2$ = obs1$.pipe(
    first()
)
obs2$.subscribe(data=>console.log(data))
```

