require 'rubygems'
require 'rake'

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name = "on_the_spot"
    gem.summary = %Q{unobtrusive in place editing}
    gem.description = %Q{Unobtrusive in place editing, using jEditable; only works in Rails 3}
    gem.email = "nathan@dixis.com"
    gem.homepage = "http://github.com/nathanvda/on_the_spot"
    gem.authors = ["Nathan Van der Auwera"]
    gem.add_development_dependency "rspec", ">= 2.0.0.beta20"
    # gem is a Gem::Specification... see http://www.rubygems.org/read/chapter/20 for additional settings
  end
  Jeweler::GemcutterTasks.new
rescue LoadError
  puts "Jeweler (or a dependency) not available. Install it with: gem install jeweler"
end

require 'rake/rdoctask'
Rake::RDocTask.new do |rdoc|
  version = File.exist?('VERSION') ? File.read('VERSION') : ""

  rdoc.rdoc_dir = 'rdoc'
  rdoc.title = "on_the_spot #{version}"
  rdoc.rdoc_files.include('README*')
  rdoc.rdoc_files.include('lib/**/*.rb')
end
