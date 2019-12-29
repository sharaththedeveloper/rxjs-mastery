# Reduce

> works similar to Array reduce

``` javascript
import { reduce } from "rxjs/operators";
import { of } from "rxjs";

const obs1 = of(1,2,3,4);
obs1.pipe(reduce((acc,cur)=>acc+cur,0))
.subscribe(data=>console.log(data),error=>console.log(error))
```

