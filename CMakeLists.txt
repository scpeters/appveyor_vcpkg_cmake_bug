cmake_minimum_required(VERSION 3.5.1 FATAL_ERROR)
cmake_policy(GET CMP0048 policy)
message(STATUS "CMP0048 policy: ${policy}")

find_package(ignition-cmake0 REQUIRED)

# the following line causes an error when used with appveyor
# and the recommended vcpkg toolchain file
project(appveyor_vcpkg_cmake_bug VERSION 0.1.0)
