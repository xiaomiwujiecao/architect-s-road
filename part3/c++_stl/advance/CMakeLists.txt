add_executable(cpp_files_streams cpp_files_streams.cpp)
add_executable(read read.cpp)
add_executable(cpp_exceptions_handling_a cpp_exceptions_handling_a.cpp)
add_executable(cpp_exceptions_handling_b cpp_exceptions_handling_b.cpp)
add_executable(cpp_dynamic_memory cpp_dynamic_memory.cpp)
add_executable(cpp_dynamic_memory_a cpp_dynamic_memory_a.cpp)
add_executable(cpp_namespaces_a cpp_namespaces_a.cpp)
add_executable(cpp_namespaces_b cpp_namespaces_b.cpp)
add_executable(cpp_namespace_c cpp_namespace_c.cpp)
add_executable(cpp_namespace_d cpp_namespace_d.cpp)
add_executable(cpp_templates_a cpp_templates_a.cpp)
add_executable(cpp_templates_b cpp_templates_b.cpp)
add_executable(cpp_preprocessor_a cpp_preprocessor_a.cpp)
add_executable(cpp_preprocessor_b cpp_preprocessor_b.cpp)
add_executable(cpp_preprocessor_c cpp_preprocessor_c.cpp)
add_executable(cpp_signal_handling_a cpp_signal_handling_a.cpp)
add_executable(cpp_signal_handling_b cpp_signal_handling_b.cpp)
add_executable(cpp_multithreading_a cpp_multithreading_a.cpp)
add_executable(cpp_multithreading_b cpp_multithreading_b.cpp)
add_executable(cpp_multithreading_c cpp_multithreading_c.cpp)
add_executable(server server.cpp)
add_executable(cgi_env cgi_env.cpp)
add_executable(cgi_lib_a cgi_lib_a.cpp)

set(INC_DIR /usr/local/include/)
set(INC_LIB /usr/local/lib/)
add_library(advance cpp_files_streams.cpp read.cpp cpp_exceptions_handling_a.cpp cpp_dynamic_memory.cpp cpp_namespaces_a.cpp cpp_namespace_c.cpp cpp_templates_a.cpp cpp_preprocessor_a.cpp cpp_preprocessor_b.cpp cpp_signal_handling_a.cpp cpp_multithreading_a.cpp server.cpp cgi_env.cpp cgi_lib_a.cpp)
include_directories(${CMAKE_CURRENT_BINARY_DIR})
include_directories(${INC_DIR})
include_directories(${INC_LIB})
install(TARGETS advance DESTINATION bin)
install(FILES cpp_files_streams.cpp DESTINATION include)
