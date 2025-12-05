project(
  'farser',
  ['fortran'],
  version: run_command(meson.current_source_dir()/'version.sh', check: true).stdout().strip(),
  meson_version: '>=1.2'
)

meson.add_dist_script('version.sh')

# Subdirectories
subdir('src')
subdir('test')

