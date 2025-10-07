cmake_minimum_required(VERSION 3.10)

project(argon2)

add_library(argon2_lib STATIC
    src/argon2.c
    src/core.c
    src/blake2/blake2b.c
    src/thread.c
    src/encoding.c
    src/ref.c
)

target_include_directories(argon2_lib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)
