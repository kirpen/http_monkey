require "bundler/gem_tasks"
require "rake/testtask"

ENV["RUBYOPT"] = "rubygems" if ENV["RUBYOPT"].nil?

Rake::TestTask.new do |t|
  t.libs.push "lib"
  t.libs.push "test"
  t.test_files = FileList['test/**/*_test.rb']
  t.verbose = true
end

task :default => :test
