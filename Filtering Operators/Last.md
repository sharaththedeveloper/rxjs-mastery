# Last

> subscribes to last emmited value from the observable

``` javascript
import { of } from "rxjs";
import { last } from "rxjs/operators";
const obs1$ = of(1,2,3,4,5,6,7,8,9,10);
const obs2$ = obs1$.pipe(
    last()
)
obs2$.subscribe(data=>console.log(data))
```

