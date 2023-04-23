add_executable(elf2rel
  elf2rel.cpp
  elf2rel.h
)

target_include_directories( elf2rel PRIVATE
  ${CMAKE_CURRENT_LIST_DIR})

find_package(Boost REQUIRED COMPONENTS program_options)
target_link_libraries(elf2rel Boost::program_options )
