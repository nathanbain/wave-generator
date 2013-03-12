require 'active_support/dependencies'

namespace :wave do
  ActiveSupport::Dependencies.autoload_paths << File.expand_path(File.join(Dir.pwd, 'lib'))
  ENV['URL'].nil? ? url_to_assess = "http://www.w3.org/" : url_to_assess = ENV['URL']

  task :make do
    WaveGenerator.new(url_to_assess, :all).make_waves
  end

  task :make_errors do
    WaveGenerator.new(url_to_assess, :errors).make_waves
  end

  task :make_errors_and_features do
    WaveGenerator.new(url_to_assess, :errors_and_features).make_waves
  end
end
