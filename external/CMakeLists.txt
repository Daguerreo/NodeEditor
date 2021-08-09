if(BUILD_TESTING)
    if(NOT TARGET Catch2)
        find_package(Catch2 2.3.0 QUIET)
    endif()

    if(NOT Catch2_FOUND)
        add_subdirectory(Catch2)
    endif()
endif()
