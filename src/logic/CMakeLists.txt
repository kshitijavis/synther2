set(LOGIC_SOURCES
    "note.cc"
    "key.cc"
)
set(LOGIC_HEADERS
    ${synther_SOURCE_DIR}/include/logic/note.h
    ${synther_SOURCE_DIR}/include/logic/key.h
)
message(${LOGIC_HEADERS})

add_library(${LOGIC_LIBRARY_NAME} STATIC
    ${LOGIC_SOURCES}
    ${LOGIC_HEADERS}
)

target_include_directories(${LOGIC_LIBRARY_NAME} PUBLIC ${synther_SOURCE_DIR}/include)