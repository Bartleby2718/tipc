add_library(prettyprint)
target_sources(prettyprint
        PUBLIC
        ${CMAKE_CURRENT_SOURCE_DIR}/PrettyPrinter.cpp
        ${CMAKE_CURRENT_SOURCE_DIR}/PrettyPrinter.h
        )
target_include_directories(prettyprint
        PUBLIC
        ${CMAKE_SOURCE_DIR}/src/frontend/ast
        ${CMAKE_SOURCE_DIR}/src/frontend/ast/treetypes
        )
target_link_libraries(prettyprint coverage_config)

