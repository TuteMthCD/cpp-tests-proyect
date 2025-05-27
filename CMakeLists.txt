cmake_minimum_required(VERSION 3.13)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

project(tests)

enable_testing()


# Usar GoogleTest ya instalado
find_package(GTest REQUIRED)

# Ejecutable de tests
add_executable(tests
    tests.cpp
)

target_include_directories(tests PRIVATE ../libs)
target_link_libraries(tests GTest::GTest GTest::Main)

include(GoogleTest)
gtest_discover_tests(tests)
