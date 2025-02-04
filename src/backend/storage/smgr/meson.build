# Copyright (c) 2022-2025, PostgreSQL Global Development Group

backend_sources += files(
  'bulk_write.c',  
  'smgr.c',
)

inc_dir = include_directories('../../../../src/include', '../../../../src/include/utils' )
md_smgr_files = files('md.c', '../file/fd.c', '../../../../src/include/utils/elog.h', '../../../../src/backend/utils/error/elog.c' )
md_smgr_lib = shared_module('md-smgr', md_smgr_files, include_directories: inc_dir, install:true, install_dir: get_option('libdir')/'postgresql')


