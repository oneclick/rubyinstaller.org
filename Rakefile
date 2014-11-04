begin
  require "bundler/setup"
rescue LoadError
  abort "Please `gem install bundler` first."
end

namespace :assets do
  desc "Compile Sass assets"
  task :compile do
    # FIXME: allow other css files?
    sh "sass themes/rubyinstaller/source/sass/main.scss:themes/rubyinstaller/static/css/main.css"
  end

  desc "Watch for Sass changes and compile again"
  task :watch do
    sh "sass --watch themes/rubyinstaller/source/sass:themes/rubyinstaller/static/css"
  end
end

desc "Generate site"
task :build => [:hugo] do
  sh "hugo"
end

task :default => [:build]

desc "Obtain Hugo executable for your platform"
task :hugo do
  # TODO
end

desc "Build site localy and watch for modifications"
task :preview => [:hugo] do
  exec "hugo server --buildDrafts --buildFuture --watch"
end
