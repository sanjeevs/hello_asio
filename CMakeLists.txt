cmake_minimum_required(VERSION 3.5)

project (Hello)
set(CMAKE_CXX_STANDARD 14)

set(THREADS_PREFER_PTHREAD_FLAG ON)
find_package(Threads REQUIRED)

# For debugging boost do the following
# set(Boost_DEBUG ON)
 set(Boost_USE_STATIC_LIBS ON)

find_package("Boost" REQUIRED COMPONENTS system chrono unit_test_framework)
include_directories(${Boost_INCLUDE_DIRS})
link_directories(${Boost_LIBRARY_DIR})

add_subdirectory(src)

enable_testing()
add_subdirectory(tests)