cmake_minimum_required(VERSION 2.8)
project(cmake-test)

configure_file(config.in config @ONLY)
add_custom_target(config ALL)
set_directory_properties(PROPERTIES
  ADDITIONAL_MAKE_CLEAN_FILES "config")
