set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -pthread")

set(SAMPLE_NAME "uuidgen")

set(LOCAL_SRCS "")
aux_source_directory(src LOCAL_SRCS)

add_executable( ${SAMPLE_NAME} ${LOCAL_SRCS} )
target_link_libraries( ${SAMPLE_NAME} PocoFoundation )
