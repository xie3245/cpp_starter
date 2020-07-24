# Generic test that uses conan libs
add_executable(cppstarter main.cpp)
target_link_libraries(
  cppstarter
  PRIVATE project_options
          project_warnings
          CONAN_PKG::fmt
          CONAN_PKG::spdlog)
