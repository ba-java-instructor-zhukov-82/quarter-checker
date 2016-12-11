##Quarter Checker

<span>A simple JavaScript project which allows
to identify a point quarter based on 
input values of its 'x' and 'y' axis.</span> 

Here is its code:  

```javascript
if(isNaN(x) || isNaN(y)) {
    print('Some coordinate was passed with incorrect value!');
}

if(x == '' || y == '') {
    print('Some coordinate value is empty!');
} else if(x > 0 && y > 0) {
    print('Point is in 1st QUARTER!');
} else if(x < 0 && y > 0) {
    print('Point is in 2nd QUARTER!');
} else if(x < 0 && y < 0) {
    print('Point is in 3rd QUARTER!');
} else if(x > 0 && y < 0) {
    print('Point is in 4th QUARTER!');
} else if(x == 0 && y > 0) {
    print('Point is in 1st or in 2nd QUARTER!');
} else if(x == 0 && y < 0) {
    print('Point is in 2nd or in 3rd QUARTER!');
} else if(x < 0 && y == 0) {
    print('Point is in 3rd or in 4th QUARTER!');
} else if(x > 0 && y == 0) {
    print('Point is in 1st or in 4th QUARTER!');
} else if(x == 0 && y == 0) {
    print('Point is in beginning of coordinate system!');
}
```