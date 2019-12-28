# FromEvent

> used to create observable from DOM events

``` javascript
import { fromEvent } from 'rxjs';

const target = document.getElementById('btn');
const obs$ = fromEvent(target,'click');
obs$.subscibe(data=>console.log(data))
```

