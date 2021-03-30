add_executable(
  main_test
  doctest_main.cpp
  example_test.cpp
  )
doctest_discover_tests(main_test ADD_LABELS 1)
target_link_libraries(
  main_test
  doctest::doctest
  )
