# Minimal doctest
A minimal project the uses CMake to install and use doctest

This project has no dependencies this shows how to use CMake to fetch doctest. It also shows how to automatically configure tests.

# Building
```
mkdir build
cd build
cmake .. # (-G Ninja) to use Ninja
make # (or Ninja)
ctest 
ctest -L Unit Tests # we label tests automatically!
```
