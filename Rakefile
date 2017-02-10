require 'rubygems'
require 'opal'
require 'opal-browser'
require 'hyper-react'
require 'opal-jquery'

desc 'Build hyperloop-express.js'
task :build do
  Opal.append_path 'hyperloop-express'
  File.binwrite 'hyperloop-express.js', Opal::Builder.build('application').to_s
end

task default: [:build]
