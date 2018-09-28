task :environment do
  require_relative  'config/environment.rb'
end


namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'puts hello to the terminal'
  task :hola do
    puts "hola de Rake!"
  end
end

namespace :db do
  desc 'invokes enviroment dependancy and creates students table'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'dummy data seed'
  task :seed do
    require_relative './db/seeds.rb'
  end
end
