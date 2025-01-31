
cmake_minimum_required(VERSION 3.12)

# Pull in PICO SDK (must be before project)
include(../pico_sdk_import.cmake)

project(pico-tflmicro-test C CXX ASM)
set(CMAKE_C_STANDARD 11)
set(CMAKE_CXX_STANDARD 11)

pico_sdk_init()

add_subdirectory("greedy_memory_planner_test")
add_subdirectory("kernel_activations_test")
add_subdirectory("kernel_add_test")
add_subdirectory("kernel_arg_min_max_test")
add_subdirectory("kernel_ceil_test")
add_subdirectory("kernel_circular_buffer_test")
add_subdirectory("kernel_comparisons_test")
add_subdirectory("kernel_concatenation_test")
add_subdirectory("kernel_conv_test")
add_subdirectory("kernel_depthwise_conv_test")
add_subdirectory("kernel_dequantize_test")
add_subdirectory("kernel_detection_postprocess_test")
add_subdirectory("kernel_elementwise_test")
add_subdirectory("kernel_floor_test")
add_subdirectory("kernel_fully_connected_test")
add_subdirectory("kernel_hard_swish_test")
add_subdirectory("kernel_l2norm_test")
add_subdirectory("kernel_logical_test")
add_subdirectory("kernel_logistic_test")
add_subdirectory("kernel_maximum_minimum_test")
add_subdirectory("kernel_mul_test")
add_subdirectory("kernel_neg_test")
add_subdirectory("kernel_pack_test")
add_subdirectory("kernel_pad_test")
add_subdirectory("kernel_pooling_test")
add_subdirectory("kernel_prelu_test")
add_subdirectory("kernel_quantization_util_test")
add_subdirectory("kernel_quantize_test")
add_subdirectory("kernel_reduce_test")
add_subdirectory("kernel_reshape_test")
add_subdirectory("kernel_resize_nearest_neighbor_test")
add_subdirectory("kernel_round_test")
add_subdirectory("kernel_shape_test")
add_subdirectory("kernel_softmax_test")
add_subdirectory("kernel_split_test")
add_subdirectory("kernel_split_v_test")
add_subdirectory("kernel_strided_slice_test")
add_subdirectory("kernel_sub_test")
add_subdirectory("kernel_svdf_test")
add_subdirectory("kernel_tanh_test")
add_subdirectory("kernel_unpack_test")
add_subdirectory("linear_memory_planner_test")
add_subdirectory("memory_arena_threshold_test")
add_subdirectory("memory_helpers_test")
add_subdirectory("micro_allocator_test")
add_subdirectory("micro_error_reporter_test")
add_subdirectory("micro_interpreter_test")
add_subdirectory("micro_mutable_op_resolver_test")
add_subdirectory("micro_string_test")
add_subdirectory("micro_time_test")
add_subdirectory("micro_utils_test")
add_subdirectory("recording_micro_allocator_test")
add_subdirectory("recording_simple_memory_allocator_test")
add_subdirectory("simple_memory_allocator_test")
add_subdirectory("testing_helpers_test")
