# Distinct Until Changed

> filter out similar emitted values

``` javascript
import { of } from "rxjs";
import { distinctUntilChanged } from "rxjs/operators";
const obs1$ = of(1,1,1,1,1,2);
const obs2$ = obs1$.pipe(
    distinctUntilChanged()
)
obs2$.subscribe(data=>console.log(data))
```

