https://leetcode.com/problems/flipping-an-image/
```

var flipAndInvertImage = function(A) {
    A.forEach(row => {
        row.reverse();
        row.forEach((el, index) => {
            if(el === 1) {
                row[index] = 0
            } else row[index] = 1
        })
    });
    return A;
};
```
