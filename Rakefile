require 'rubocop/rake_task'

desc 'Run Rubocop on the code'
RuboCop::RakeTask.new(:rubocop) do |task|
  task.fail_on_error = true
end

desc 'Build the site'
task :build do
  raise unless system 'jekyll build'
end

task default: %i[rubocop build]
