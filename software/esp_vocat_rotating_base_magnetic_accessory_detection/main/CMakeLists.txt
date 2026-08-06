idf_component_register(SRCS "echoear_rotating_base_main.c"
                    INCLUDE_DIRS ".")

if(MAG_SW_PROFILE STREQUAL "base")
    target_compile_definitions(${COMPONENT_LIB} PRIVATE MAG_SW_PROFILE_BASE=1)
endif()
