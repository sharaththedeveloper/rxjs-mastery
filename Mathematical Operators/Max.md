# Max

> return the maximum value emitted from an observable

``` javascript
import { max } from "rxjs/operators";
import { of } from "rxjs";

const obs1 = of(1,2,3,4);
obs1.pipe(max()).subscribe(data=>console.log(data),error=>console.log(error))
```

