src = [
  'fparser.f90',
  'parameters.f90',
]

fparser_lib = static_library(
  'fparser',       # genera libfparser.a
  src,
  pic: true,       # evita TEXTREL/PIE issues
  install: true,
)
          
# Exportar dependencia para que otros (tests o ejecutables) puedan linkearla
fparser_dep = declare_dependency(
  link_with: fparser_lib,
  include_directories: include_directories('.')
)
