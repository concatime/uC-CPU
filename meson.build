uccpu_deps = []
uccpu_inc = include_directories('.', architecture / compiler)
uccpu_src = files('cpu_core.c')
if get_variable('default_configuration', false)
  uccpu_inc = [uccpu_inc, include_directories('Cfg/Template')]
  uccpu_src += files('BSP/Template/bsp_cpu.c')
endif
subdir(architecture / compiler)
