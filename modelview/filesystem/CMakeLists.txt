add_executable(filesystem
"main.cpp" )

target_link_libraries(filesystem PRIVATE Qt${QT_VERSION_MAJOR}::Widgets)

set_target_properties(filesystem PROPERTIES
          CXX_STANDARD 17
          #CXX_EXTENSIONS OFF
          )