demo_vkd3d_deps = [
  threads_dep, vkd3d_common_dep
]

if vkd3d_platform != 'windows'
  demo_vkd3d_deps += [
    lib_m,
    lib_xcb,
    lib_xcbkeysyms,
    lib_d3d12
  ]
else
  demo_vkd3d_deps += [
    lib_dxgi,
    lib_d3d12
  ]
endif

executable('gears', 'gears.c',
  dependencies        : demo_vkd3d_deps,
  include_directories : vkd3d_public_includes,
  install             : true,
  gui_app             : true)

executable('triangle', 'triangle.c',
  dependencies        : demo_vkd3d_deps,
  include_directories : vkd3d_public_includes,
  install             : true,
  gui_app             : true)
