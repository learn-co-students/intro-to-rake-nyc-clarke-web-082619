namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end
  desc 'outputs hello in spanish to the terminal'
  task :hola do
    puts 'hola de Rake!'
  end
end

desc 'makesure the method exists'
task :console do
end

namespace :db do
  desc 'migrate changes to database'
  task :migrate => :environment do 
    Student.create_table
  end

  task :environment do
    require_relative './config/environment'
  end

  desc 'seeds the database with dummy data from seed file'
  task :seed do 
    require './db/seeds.rb'
  end
end

