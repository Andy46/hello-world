cmake_minimum_required(VERSION 3.24)

set(APPNAME "hello")

project(${APPNAME})

add_executable(${APPNAME})

FILE(GLOB SRCS src/*)

target_sources(${APPNAME}
    PRIVATE ${SRCS}
)
