project(tests CXX)

add_executable(tests test.cpp)
target_link_libraries(tests source-lib)

include(CTest)
add_test(NAME tests COMMAND tests)