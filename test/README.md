cd ..

change main.c as needed

clang main.c -I./src -Os -o interp && time ./interp

gcc main.c -I./src -Os -o interp && time ./interp

example_1:
```
USE_SWITCH
real    0m1.476s

USE_DTC
real    0m0.838s

USE_TTC
real    0m0.860s

USE_TAIL_CALLS
real    0m0.868s

USE_CALLS
real    0m2.297s

USE_INLINE
real    0m0.099s
```
