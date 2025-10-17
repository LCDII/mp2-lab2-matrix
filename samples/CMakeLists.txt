set(target "Matrix_sample")

file(GLOB hdrs "*.h*")
file(GLOB srcs "*.cpp*")
file(GLOB matrix "${CMAKE_CURRENT_SOURCE_DIR}/tmatrix.h")


add_executable(${target} ${srcs} ${hdrs} ${matrix})

target_link_libraries(${target} ${MP2_LIBRARY})