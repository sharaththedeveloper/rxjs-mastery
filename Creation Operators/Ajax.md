# Ajax

> Ajax is used to make HTTP request to server

**Code**

*HTTP GET request*

```javascript
import { ajax } from 'rxjs/ajax';
import { of } from 'rxjs';
import { catchError, map } from "rxjs/operators";

const obs$ = ajax('https://jsonplaceholder.typicode.com/users').pipe(
map(userResponse => userResponse.response),
catchError(err => of(err))
);
obs$.subscribe(data=>console.log(data))

```

*HTTP POST request*

``` javascript
import { ajax } from 'rxjs/ajax';
import { of } from 'rxjs';
import { catchError, map } from "rxjs/operators";

const obs$ = ajax({url : 'https://jsonplaceholder.typicode.com/users', method:'POST', data:{'users':'sharath'}}).pipe(
map(userResponse => userResponse.response),
catchError(err => of(err))
);
obs$.subscribe(data=>console.log(data))
```



