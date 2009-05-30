require 'rubygems'
require 'rake/gempackagetask'
PKG_NAME = "filemanager"
PKG_VERSION = "0.3.1"
PKG_FILE_NAME = "#{PKG_NAME}-#{PKG_VERSION}"
PKG_FILES = FileList[
  '[A-Z]*',
  'lib/**/*',
  'filemanager/**/*'
]
spec = Gem::Specification.new do |s|
  s.platform = Gem::Platform::RUBY
  s.summary = "A online file manager for rails project"
  s.name = PKG_NAME
  s.version = PKG_VERSION
  s.require_path = 'lib'
  s.homepage = %q{http://filemanager.rubyforge.org/}
  s.rubyforge_project = 'Filemanager'
  s.has_rdoc = false
  s.authors = ["Leon Li"]
  s.email = "scorpio_leon@hotmail.com"
  s.files = PKG_FILES
  s.description = <<-EOF
    A online file manager for rails project£¬support file/folder actions such as browse, create, rename, remove, copy, move, zip download, upload, unzip, view
  EOF
end
Rake::GemPackageTask.new(spec) do |pkg|
  pkg.need_zip = true
  pkg.need_tar = true
end
