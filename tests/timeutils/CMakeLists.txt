add_executable(timeutils_tests timeutils_tests_main.cpp)
target_link_libraries(timeutils_tests test_common libslic3r ${Boost_LIBRARIES} ${TBB_LIBRARIES} ${Boost_LIBRARIES})

add_test(timeutils_tests timeutils_tests)
#gtest_discover_tests(timeutils_tests TEST_PREFIX timeutils.)
