pulse_dep = dependency('libpulse', version: '>= 0.9.5', required: false)


if pulse_dep.found()
  shared_module('pulse_audio',
    'pulse_audio.cc',
    dependencies: [audacious_dep, pulse_dep, glib_dep],
    install: true,
    install_dir: output_plugin_dir
  )
endif

