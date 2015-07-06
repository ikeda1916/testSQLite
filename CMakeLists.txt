cmake_minimum_required(VERSION 2.8)
project(SQLitetest)

add_executable(test test.cxx)

add_library(sqlite3 SHARED sqlite3.c)

target_link_libraries(test sqlite3)

