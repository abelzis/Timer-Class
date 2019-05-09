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


Example:

```cpp
#include <iostream>
#include <vector>
#include "timerClass.h" //timer

int main()
{
  // start v1 fill time
  Timer t1;
  std::vector<int> v1;
  for (int i = 1; i <= 10000000; ++i)
    v1.push_back(i);
  t1.pause();
  // end v1 fill time
  std::cout << "std::vector<int> fill " << sz << ": " << t1.elapsed() << " s\n";
}
```

**Output**: [result](https://i.gyazo.com/924485962d5a8ae1e51e5a0a938eb967.png)

Simple structure to use. Uses `<chrono>` library for high resolution clocking (up to nanoseconds).
