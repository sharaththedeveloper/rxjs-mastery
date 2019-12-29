# Merge

>merge is used to comine two or more observables, the number of concurrent observables can also be specified

``` javascript
import { merge, range } from "rxjs";
const obs1$ = range(1,5);
const obs2$ = range(1,10);
const obs3$ = range(1,20);
const obs4$ = range(1,30);
const concurrent = 2;
const obs5$ = merge(obs1$,obs2$,obs3$,obs4$,concurrent);
obs5$.subscribe(data=>console.log(data))
```

