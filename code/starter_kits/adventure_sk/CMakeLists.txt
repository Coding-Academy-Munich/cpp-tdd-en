cmake_minimum_required(VERSION 3.20)
project(adventure_sk)

set(CMAKE_CXX_STANDARD 20)

add_subdirectory(data)

add_executable(${PROJECT_NAME}
    main.cpp
)
target_link_libraries(${PROJECT_NAME} PRIVATE adventure_sk_data)
