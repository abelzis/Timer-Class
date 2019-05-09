# Timer-Class
Timer class with pauses and resumes.

# How to use it?
Download the header, place it in your C++ program folder, include it with #include "timerClass.h". Syntax is simple:

```cpp
Timer t;      //starts timer
t.pause()     //pauses timer
t.resume()    //resumes timer
t.elapsed()   //returns time in seconds (double)
t.reset()     //resets timer
```

Simple structure to use. Uses `<chrono>` library for high resolution clocking (up to nanoseconds).
