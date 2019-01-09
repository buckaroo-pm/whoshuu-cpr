load('//:subdir_glob.bzl', 'subdir_glob')
load('//:buckaroo_macros.bzl', 'buckaroo_deps_from_package')

cxx_library(
  name = 'cpr',
  header_namespace = '',
  exported_headers = subdir_glob([
    ('include', '**/*.h'),
  ]),
  srcs = glob([
    'cpr/**/*.cpp',
  ]),
  licenses = [
    'LICENSE',
  ],
  deps = buckaroo_deps_from_package('github.com/buckaroo-pm/pkg-config-curl'),
  visibility = [
    'PUBLIC'
  ],
)
