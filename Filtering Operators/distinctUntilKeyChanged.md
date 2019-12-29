# Distinct Until Key Changed 

> similar to distinctUntilChanged except works with keys

``` javascript
import { from } from "rxjs";
import { distinctUntilKeyChanged } from "rxjs/operators";
const obs1$ = from([{name:'sharath'},{name:'sharath'},{name:'sharath'},{name:'zeref'},{name:'sharath'},{name:'sharath'}]);
const obs2$ = obs1$.pipe(
    distinctUntilKeyChanged('name')
)
obs2$.subscribe(data=>console.log(data))
```

