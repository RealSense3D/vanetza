find_package(Cohda MODULE REQUIRED)
add_executable(cohda_proxy proxy.cpp proxy_handler.cpp)
target_include_directories(cohda_proxy PUBLIC ${COHDA_INCLUDE_DIRS})
target_link_libraries(cohda_proxy Boost::system net)
