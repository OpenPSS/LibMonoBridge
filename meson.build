project('MonoBridge', 'cpp',
  version  '0.1',
  default_options  ['warning_level=3', 'cpp_std=c++14'])


cpp = meson.get_compiler('cpp')
dirbase = meson.current_source_dir()

libMonoBridge = static_library('MonoBridge',
	'PssCrypto.cpp'
	install  true)
	
libMonoBridge_dep = declare_dependency(link_with libMonoBridge)