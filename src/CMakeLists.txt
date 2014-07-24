cmake_minimum_required(VERSION 2.4)

project(ag)

add_definitions(-g -O3)

add_executable(ag
    decompress.c
    ignore.c
    lang.c
    log.c
    main.c
    options.c
    print.c
    scandir.c
    search.c
    util.c
)

target_link_libraries(ag -lpcre -lpthread -llzma -lz)
