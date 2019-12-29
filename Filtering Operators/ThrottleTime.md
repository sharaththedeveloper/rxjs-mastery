# Throttle Time

> Limits the emitted rate based on time

``` javascript
import { fromEvent } from "rxjs";
import { throttleTime } from "rxjs/operators";
const obs1$ = fromEvent(document,'click');
const obs2$ = obs1$.pipe(
    throttleTime(2000)
)
obs2$.subscribe(data=>console.log(data))
```

