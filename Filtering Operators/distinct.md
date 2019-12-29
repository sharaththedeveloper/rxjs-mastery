# Distinct

> similar to distinctUntilChanged except filters only distinct and not consecutively distinct

*Distinct values*

``` javascript
import { of } from "rxjs";
import { distinct } from "rxjs/operators";
const obs1$ = of(1,1,1,1,2,1,1,3,4);
const obs2$ = obs1$.pipe(
    distinct()
)
obs2$.subscribe(data=>console.log(data))
```

*Distinct Keys*

``` javascript
import { of } from "rxjs";
import { distinct } from "rxjs/operators";
const obs1$ = of({name:'sharath'},{name:'sharath'},{name:'sharath'},{name:'zeref'},{name:'sharath'},{name:'sharath'});
const obs2$ = obs1$.pipe(
    distinct(p=>p.name)
)
obs2$.subscribe(data=>console.log(data))
```

