project('MonoBridge', 'cpp',
  version: '0.1',
  default_options: ['warning_level=0', 'cpp_std=c++20', 'default_library=static'])


cpp = meson.get_compiler('cpp')
dirbase = meson.current_source_dir()
include_libs = include_directories('.')

libMonoBridge = static_library('MonoBridge',
	'PssCrypto.cpp',
	include_directories: [ include_libs ],
	install: true)

libMonoBridge_dep = declare_dependency(include_directories: include_libs, link_with: libMonoBridge)
