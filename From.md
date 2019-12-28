# From

> convert array to observable

``` javascript
import { from } from "rxjs";
const obs$ = from([1,2,3]);
obs$.subscribe(data=>console.log(data))
```

