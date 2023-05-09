add_executable(multiview
"createModel.cpp" "createModel.h" "multiview.cpp")

target_link_libraries(multiview PRIVATE Qt${QT_VERSION_MAJOR}::Widgets)

set_target_properties(multiview PROPERTIES
          CXX_STANDARD 17
          #CXX_EXTENSIONS OFF
          )