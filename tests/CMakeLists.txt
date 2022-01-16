add_executable(mytest test1.cpp)
target_link_libraries(mytest ${Boost_UNIT_TEST_FRAMEWORK_LIBRARY})

add_test(NAME test1 COMMAND mytest)