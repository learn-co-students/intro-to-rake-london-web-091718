

desc 'commands for greetings'
namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts 'hello from Rake!'
  end
  desc 'prints hola de rake'
  task :hola do
    puts 'hola de Rake!'
  end
end

task :environment do
  require_relative './config/environment'
end




namespace :db do
  desc 'migrate changes to your database'
  task :migrate => :environment do
    Student.create_table
  end
  desc 'seeds the database with dummy data from a seed file'
  task :seed do
    require_relative './db/seeds.rb'
  end

end
