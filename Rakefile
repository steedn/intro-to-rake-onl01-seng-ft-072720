namespace :Greeting_1 do
namespace :greeting do
desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end

desc 'outputs hola to the terminal'
task :hola do
  puts "hola de Rake!"
end
end
end

namespace :db do
  desc 'migrate changes to your database'
  task :migrate => :environment do
    Student.create_table
  end

  task :environment do
    require_relative './config/environment'
  end
  desc 'seed db with dummy data'
  task :seed do
    require_relative './db/seeds'
  end
end
