# Debounce Time

> Works similar to throttle, waits and then emits and event

``` javascript
import { fromEvent } from "rxjs";
import { debounceTime,throttleTime } from "rxjs/operators";
const obs1$ = fromEvent(document,'click');
const obs2$ = obs1$.pipe(
    debounceTime(2000)
)
obs2$.subscribe(data=>console.log(data))

```

