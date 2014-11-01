begin
  require "bundler/setup"
rescue LoadError
  abort "Please `gem install bundler` first."
end

desc "Obtain Hugo executable for your platform"
task :hugo do
  # TODO
end

desc "Build site localy and watch for modifications"
task :preview => [:hugo] do
  exec "hugo server --buildDrafts --buildFuture --watch"
end
