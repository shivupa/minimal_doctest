cmake_minimum_required(VERSION 3.14.0 FATAL_ERROR)
include(FetchContent)
project(Example)

enable_testing()

FetchContent_Declare(
  doctest
  GIT_REPOSITORY https://github.com/onqtam/doctest.git
  GIT_TAG origin/master)
FetchContent_MakeAvailable(doctest)
include(${doctest_SOURCE_DIR}/scripts/cmake/doctest.cmake)

add_subdirectory(src)
add_subdirectory(tests)
