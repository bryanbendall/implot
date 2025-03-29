add_library(implot 
                implot.cpp
                implot.h
                implot_demo.cpp
                implot_internal.h
                implot_items.cpp
            ) 

target_include_directories(implot PUBLIC
                           ${CMAKE_CURRENT_SOURCE_DIR}
                           )

target_link_libraries(implot PUBLIC 
                        imgui
                    )