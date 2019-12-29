# Concat

> executes one observable sequentially after the other

``` javascript
import { concat, range } from "rxjs";
const obs1$ = range(1,5);
const obs2$ = range(1,10);
const obs3$ = range(1,20);
const obs4$ = range(1,30);

const obs5$ = concat(obs1$,obs2$,obs3$,obs4$);
obs5$.subscribe(data=>console.log(data))
```

