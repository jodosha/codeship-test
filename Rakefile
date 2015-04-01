require 'rake'

namespace :test do
  task :models do
    sleep 8
  end

  task :controllers do
    sleep 5
  end

  task :features do
    sleep 16
  end

  task :all do
    %w(models controllers features).each do |type|
      puts task = "test:#{ type }"
      Rake::Task[task].invoke
    end
  end
end

task default: 'test:all'
