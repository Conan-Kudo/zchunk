add_global_arguments('-Wunused-result', language : 'c')
add_global_arguments('-std=gnu99', language : 'c')
subdir('lib')
executable('zck', ['zck.c', 'util_common.c', 'buzhash/buzhash.c'], include_directories: inc, link_with: zcklib, install: true)
executable('unzck', ['unzck.c', 'util_common.c'], include_directories: inc, link_with: zcklib, install: true)
executable('zckdl', ['zck_dl.c', 'util_common.c'], include_directories: inc, dependencies: curl_dep, link_with: zcklib, install: true)
executable('zck_read_header', ['zck_read_header.c', 'util_common.c'], include_directories: inc, link_with: zcklib, install: true)
executable('zck_delta_size', ['zck_delta_size.c', 'util_common.c', 'memmem.c'], include_directories: inc, link_with: zcklib, install: true)
