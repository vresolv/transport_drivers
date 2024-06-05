project(asio_libs)

set(ASIO_INCLUDE_DIR "C:/asio/include" CACHE STRING "Path to Asio root directory")

add_library(${PROJECT_NAME} INTERFACE)

target_include_directories(${PROJECT_NAME} INTERFACE
    ${ASIO_INCLUDE_DIR}
)

#target_include_directories(${PROJECT_NAME} INTERFACE
#    "$<BUILD_INTERFACE:${CMAKE_CURRENT_LIST_DIR}/include>"
#    #"$<INSTALL_INTERFACE:${CMAKE_INSTALL_INCLUDEDIR}>"
#)
