# js-filter-expression-builder
Build Dynamic Linq Filter Expressions in JavaScript

# Example Usage
```js
let fxb = new FilterExpressionBuilder();
fxb.setPage(0, 50); // set the current page index to zero, with pages of size 50
fxb.addParameter('Lastname', 'Jefferson', 'text'); // parameter types are 'text' or 'number'
fxb.sortDescending('Lastname');
let searchObject = fxb.getSearchParams();
```

Useful in conjunction with the [Data Tools](https://github.com/ThoriumStack/core-datatools) library, which has the C# model for the expression.
