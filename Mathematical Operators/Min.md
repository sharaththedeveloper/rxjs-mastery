# Min

> returns the minimum value emitted from and observable

``` javascript
import { min } from "rxjs/operators";
import { of } from "rxjs";

const obs1 = of(1,2,3,4);
obs1.pipe(min()).subscribe(data=>console.log(data),error=>console.log(error))
```

