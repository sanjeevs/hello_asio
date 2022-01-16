add_executable(timer1 timer1.cpp)
target_link_libraries(timer1 Threads::Threads boost_chrono)

add_executable(timer2 timer2.cpp)
target_link_libraries(timer2 Threads::Threads boost_chrono)

add_executable(timer3 timer3.cpp)
target_link_libraries(timer3 Threads::Threads boost_chrono)

add_executable(timer4 timer4.cpp)
target_link_libraries(timer4 Threads::Threads boost_chrono)

add_executable(udp_server udp_server.cpp)
target_link_libraries(udp_server Threads::Threads boost_chrono)

add_executable(udp_client udp_client.cpp)
target_link_libraries(udp_client Threads::Threads boost_chrono)