set(CMAKE_CXX_FLAGS "-Wno-old-style-cast")
set(CMAKE_CXX_FLAGS "-Wno-unused-variable")
set(CMAKE_CXX_FLAGS "-Wno-sign-conversion")

set(TinyUtil_SRCS TinyUtil.cpp TinyConfig.cpp TinyTimer.cpp  TinyServer.cpp  TinyClient.cpp  TinyRio.cpp TinyChart.cpp)

add_library(tinyutil ${TinyUtil_SRCS})

target_link_libraries(tinyutil pthread)