file(GLOB SOURCE_LIST CONFIGURE_DEPENDS
        "${connect4_SOURCE_DIR}/src/*.cpp")

add_library(src ${SOURCE_LIST} ${HEADER_LIST})
target_include_directories(src PUBLIC ../include)