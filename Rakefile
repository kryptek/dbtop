
begin
  require 'bones'
rescue LoadError
  abort '### Please install the "bones" gem ###'
end

task :default => 'test:run'
task 'gem:release' => 'test:run'

Bones {
  name     'dbtop'
  authors  'Alfred Moreno'
  email    'kryptek@kryptek.org'
  url      'http://github.com/kryptek'
}

