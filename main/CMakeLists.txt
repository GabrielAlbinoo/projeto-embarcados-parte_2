FILE(GLOB_RECURSE app_sources ${CMAKE_SOURCE_DIR}/main/*.c ${CMAKE_SOURCE_DIR}/lib/*.c)

idf_component_register(SRCS ${app_sources}
                       INCLUDE_DIRS ${CMAKE_SOURCE_DIR}/lib)