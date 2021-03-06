set(TEST_BIN ${CMAKE_RUNTIME_OUTPUT_DIRECTORY}/${CONFIGURATION}/Test)

#add_test(address ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/address.wast)
#add_test(binary ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/binary.wast)
add_test(block ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/block.wast)
add_test(br ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/br.wast)
add_test(break-drop ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/break-drop.wast)
add_test(br_if ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/br_if.wast)
add_test(br_table ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/br_table.wast)
add_test(call ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/call.wast)
add_test(call_indirect ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/call_indirect.wast)
add_test(comments ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/comments.wast)
add_test(conversions ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/conversions.wast)
add_test(endianness ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/endianness.wast)
add_test(exports ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/exports.wast)
add_test(f32 ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/f32.wast)
add_test(f32_cmp ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/f32_cmp.wast)
add_test(f64 ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/f64.wast)
add_test(f64_cmp ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/f64_cmp.wast)
add_test(fac ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/fac.wast)
add_test(float_exprs ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/float_exprs.wast)
add_test(float_literals ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/float_literals.wast)
add_test(float_memory ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/float_memory.wast)
add_test(float_misc ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/float_misc.wast)
add_test(forward ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/forward.wast)
add_test(func ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/func.wast)
add_test(func_ptrs ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/func_ptrs.wast)
add_test(get_local ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/get_local.wast)
add_test(i32 ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/i32.wast)
add_test(i64 ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/i64.wast)
#add_test(imports ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/imports.wast)
add_test(int_exprs ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/int_exprs.wast)
add_test(int_literals ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/int_literals.wast)
add_test(labels ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/labels.wast)
add_test(left-to-right ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/left-to-right.wast)
add_test(loop ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/loop.wast)
add_test(memory ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/memory.wast)
add_test(memory_redundancy ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/memory_redundancy.wast)
add_test(memory_trap ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/memory_trap.wast)
add_test(names ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/names.wast)
add_test(nan-propagation ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/nan-propagation.wast)
add_test(nop ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/nop.wast)
#add_test(resizing ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/resizing.wast)
add_test(return ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/return.wast)
add_test(select ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/select.wast)
add_test(set_local ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/set_local.wast)
add_test(start ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/start.wast)
add_test(store_retval ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/store_retval.wast)
add_test(switch ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/switch.wast)
add_test(traps ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/traps.wast)
add_test(typecheck ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/typecheck.wast)
add_test(unreachable ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/unreachable.wast)

add_test(f32.load32.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/f32.load32.fail.wast)
set_tests_properties(f32.load32.fail PROPERTIES WILL_FAIL TRUE)

add_test(f32.load64.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/f32.load64.fail.wast)
set_tests_properties(f32.load64.fail PROPERTIES WILL_FAIL TRUE)

add_test(f32.store32.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/f32.store32.fail.wast)
set_tests_properties(f32.store32.fail PROPERTIES WILL_FAIL TRUE)

add_test(f32.store64.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/f32.store64.fail.wast)
set_tests_properties(f32.store64.fail PROPERTIES WILL_FAIL TRUE)

add_test(f64.load32.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/f64.load32.fail.wast)
set_tests_properties(f64.load32.fail PROPERTIES WILL_FAIL TRUE)

add_test(f64.load64.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/f64.load64.fail.wast)
set_tests_properties(f64.load64.fail PROPERTIES WILL_FAIL TRUE)

add_test(f64.store32.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/f64.store32.fail.wast)
set_tests_properties(f64.store32.fail PROPERTIES WILL_FAIL TRUE)

add_test(f64.store64.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/f64.store64.fail.wast)
set_tests_properties(f64.store64.fail PROPERTIES WILL_FAIL TRUE)

add_test(func-local-after-body.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/func-local-after-body.fail.wast)
set_tests_properties(func-local-after-body.fail PROPERTIES WILL_FAIL TRUE)

add_test(func-local-before-param.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/func-local-before-param.fail.wast)
set_tests_properties(func-local-before-param.fail PROPERTIES WILL_FAIL TRUE)

add_test(func-local-before-result.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/func-local-before-result.fail.wast)
set_tests_properties(func-local-before-result.fail PROPERTIES WILL_FAIL TRUE)

add_test(func-param-after-body.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/func-param-after-body.fail.wast)
set_tests_properties(func-param-after-body.fail PROPERTIES WILL_FAIL TRUE)

add_test(func-result-after-body.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/func-result-after-body.fail.wast)
set_tests_properties(func-result-after-body.fail PROPERTIES WILL_FAIL TRUE)

add_test(func-result-before-param.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/func-result-before-param.fail.wast)
set_tests_properties(func-result-before-param.fail PROPERTIES WILL_FAIL TRUE)

add_test(if_label_scope.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/if_label_scope.fail.wast)
set_tests_properties(if_label_scope.fail PROPERTIES WILL_FAIL TRUE)

add_test(i32.load32_s.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/i32.load32_s.fail.wast)
set_tests_properties(i32.load32_s.fail PROPERTIES WILL_FAIL TRUE)

add_test(i32.load32_u.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/i32.load32_u.fail.wast)
set_tests_properties(i32.load32_u.fail PROPERTIES WILL_FAIL TRUE)

add_test(i32.load64_s.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/i32.load64_s.fail.wast)
set_tests_properties(i32.load64_s.fail PROPERTIES WILL_FAIL TRUE)

add_test(i32.load64_u.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/i32.load64_u.fail.wast)
set_tests_properties(i32.load64_u.fail PROPERTIES WILL_FAIL TRUE)

add_test(i32.store32.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/i32.store32.fail.wast)
set_tests_properties(i32.store32.fail PROPERTIES WILL_FAIL TRUE)

add_test(i32.store64.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/i32.store64.fail.wast)
set_tests_properties(i32.store64.fail PROPERTIES WILL_FAIL TRUE)

add_test(i64.load64_s.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/i64.load64_s.fail.wast)
set_tests_properties(i64.load64_s.fail PROPERTIES WILL_FAIL TRUE)

add_test(i64.load64_u.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/i64.load64_u.fail.wast)
set_tests_properties(i64.load64_u.fail PROPERTIES WILL_FAIL TRUE)

add_test(i64.store64.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/i64.store64.fail.wast)
set_tests_properties(i64.store64.fail PROPERTIES WILL_FAIL TRUE)

add_test(of_string-overflow-hex-u32.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/of_string-overflow-hex-u32.fail.wast)
set_tests_properties(of_string-overflow-hex-u32.fail PROPERTIES WILL_FAIL TRUE)

add_test(of_string-overflow-hex-u64.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/of_string-overflow-hex-u64.fail.wast)
set_tests_properties(of_string-overflow-hex-u64.fail PROPERTIES WILL_FAIL TRUE)

add_test(of_string-overflow-s32.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/of_string-overflow-s32.fail.wast)
set_tests_properties(of_string-overflow-s32.fail PROPERTIES WILL_FAIL TRUE)

add_test(of_string-overflow-s64.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/of_string-overflow-s64.fail.wast)
set_tests_properties(of_string-overflow-s64.fail PROPERTIES WILL_FAIL TRUE)

add_test(of_string-overflow-u32.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/of_string-overflow-u32.fail.wast)
set_tests_properties(of_string-overflow-u32.fail PROPERTIES WILL_FAIL TRUE)

add_test(of_string-overflow-u64.fail ${TEST_BIN} ${CMAKE_CURRENT_LIST_DIR}/of_string-overflow-u64.fail.wast)
set_tests_properties(of_string-overflow-u64.fail PROPERTIES WILL_FAIL TRUE)
