# Skip

> Subscribes after specified specified value

``` javascript
import { of } from "rxjs";
import { skip } from 'rxjs/operators';

const obs1$ = of(1,2,3,4,5)
const obs2$ = obs1$.pipe(
    skip(3)
)
obs2$.subscribe(data=>console.log(data))
```

