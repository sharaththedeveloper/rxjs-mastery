# Interval

> Emits a sequential numbers periodically

``` javascript
import { interval } from "rxjs";

const obs$ = interval(1000);

obs$.subscribe(data=>console.log(data))
```

