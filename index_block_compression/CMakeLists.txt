add_executable(index_block_test index_block_test.cc)
target_link_libraries(index_block_test ${ROCKSDB_LIB} ${THIRDPARTY_LIBS} testharness gtest)
add_executable(basic_test basic_test.cc)
target_link_libraries(basic_test ${ROCKSDB_LIB} ${THIRDPARTY_LIBS})
add_executable(filter_experiment_leco filter_experiment.cc)
target_link_libraries(filter_experiment_leco ${ROCKSDB_LIB} ${THIRDPARTY_LIBS})
add_executable(filter_experiment_base filter_experiment_base.cc)
target_link_libraries(filter_experiment_base ${ROCKSDB_LIB} ${THIRDPARTY_LIBS})
add_executable(filter_experiment_int filter_experiment_int.cc)
target_link_libraries(filter_experiment_int ${ROCKSDB_LIB} ${THIRDPARTY_LIBS})
add_executable(index_block_ra index_block_random_access.cc)
target_link_libraries(index_block_ra ${ROCKSDB_LIB} ${THIRDPARTY_LIBS} gmp gmpxx)
add_executable(index_block_ra_base index_block_random_access_baseline.cc)
target_link_libraries(index_block_ra_base ${ROCKSDB_LIB} ${THIRDPARTY_LIBS} testharness gtest)