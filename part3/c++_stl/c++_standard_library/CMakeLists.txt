
add_library(c++_standard_library cpp_allocate_shared.cpp functional.cpp cpp_make_shared.cpp static_pointer_cast.cpp cpp_dynamic_pointer_cast.cpp cpp_const_pointer_cast.cpp cpp_get_deleter.cpp cpp_owner_less.cpp cpp_enable_shared_from_this.cpp cpp_new_operator_new.cpp cpp_new_bad_alloc.cpp bad_array_new_length.cpp cpp_new_operator_new_operator.cpp cpp_new_operator_operator_delete_operator.cpp cpp_new_nothrow.cpp)
include_directories(${CMAKE_CURRENT_BINARY_DIR})
install(TARGETS c++_standard_library  DESTINATION bin)
install(FILES  DESTINATION include)
add_executable(functional functional.cpp)
add_executable(cpp_make_shared cpp_make_shared.cpp)
add_executable(cpp_allocate_shared cpp_allocate_shared.cpp)
add_executable(static_pointer_cast static_pointer_cast.cpp)
add_executable(cpp_dynamic_pointer_cast cpp_dynamic_pointer_cast.cpp)
add_executable(cpp_const_pointer_cast cpp_const_pointer_cast.cpp)
add_executable(cpp_get_deleter cpp_get_deleter.cpp)
add_executable(cpp_owner_less cpp_owner_less.cpp)
add_executable(cpp_enable_shared_from_this cpp_enable_shared_from_this.cpp)
add_executable(cpp_new_operator_new cpp_new_operator_new.cpp)
add_executable(cpp_new_bad_alloc cpp_new_bad_alloc.cpp)
add_executable(bad_array_new_length bad_array_new_length.cpp)
add_executable(cpp_new_operator_new_operator cpp_new_operator_new_operator.cpp)
add_executable(cpp_new_operator_operator_delete_operator cpp_new_operator_operator_delete_operator.cpp)
add_executable(cpp_new_nothrow cpp_new_nothrow.cpp)