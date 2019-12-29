# Count

> Return an observable os the number of values emitted

``` javascript

import { count } from "rxjs/operators";
import { of } from "rxjs";

const obs1 = of(1,2,3,4);
obs1.pipe(count()).subscribe(data=>console.log(data),error=>console.log(error))
```

