file(GLOB_RECURSE CPPS  ./*.cpp )
file(GLOB_RECURSE HS  ./*.h )

add_executable(playlists ${CPPS} ${HS} mainwindow.ui)

target_link_libraries(playlists PRIVATE Qt${QT_VERSION_MAJOR}::Widgets)

set_target_properties(playlists PROPERTIES
          CXX_STANDARD 17
          #CXX_EXTENSIONS OFF
          )