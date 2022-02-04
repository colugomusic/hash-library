set(files
    ${CMAKE_CURRENT_SOURCE_DIR}/crc32.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/digest.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/keccak.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/md5.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/sha1.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/sha3.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/sha256.cpp
)

target_sources(sync PRIVATE ${files})