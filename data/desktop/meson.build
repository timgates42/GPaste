untranslated_desktop_file = configure_file(
  input: 'org.gnome.GPaste.Ui.desktop.in.in',
  configuration: conf,
  output: 'org.gnome.GPaste.Ui.desktop.in',
)

i18n.merge_file(
  'gpaste-desktop-file',
  input: untranslated_desktop_file,
  po_dir: gpaste_po_dir,
  type: 'desktop',
  output: 'org.gnome.GPaste.Ui.desktop',
  install: true,
  install_dir: join_paths(get_option('datadir'), 'applications'),
)