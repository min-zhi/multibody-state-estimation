project(ex_four_bars)

include_directories(${SPARSEMBS_INCLUDE_DIRS})
link_directories(${SPARSEMBS_LIB_DIRS})

add_executable(${PROJECT_NAME} main.cpp)
target_link_libraries(${PROJECT_NAME} ${MRPT_LIBS} ${SPARSEMBS_LIBS})
add_dependencies(${PROJECT_NAME} ${DEPENCENCIES_SPARSEMBS})
set_target_properties(${PROJECT_NAME} PROPERTIES FOLDER "Examples")
