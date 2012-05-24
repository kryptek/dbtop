dbtop
===========

Similar to the Unix 'top' tool, this Ruby gem will provide process
monitoring for your MySQL database instance.

By using command line arguments or environmental variables, dbtop will
connect to your db and return your current process list (minus Sleep
processes) on screen, in a terminal Curses buffer.

By default, the port used will be 3306 unless the environment
variable for MYSQL_PORT is specified.

Features
--------

Easy out-of-the-box connectivity to your database if you use
environmental variables.

Won't make a mess of your terminal (drawn to a Curses buffer).

Examples
--------

If you don't have environmental variables set for your MySQL database,
run dbtop with command line arguments:

```bash
  ruby dbtop.rb -u #{user} -p #{pass} -h #{host} -d #{database}
```

If you have environmental variables set for your MySQL database already,
just run dbtop :)

```bash
  ruby dbtop.rb
```

Requirements
------------

Ruby 1.9.2+

If you're using ENV variables:

MYSQL_USER
MYSQL_PASSWORD
MYSQL_HOST
MYSQL_DATABASE
MYSQL_PORT

Install
-------

Install all required gems by running:

```bash
bundle install
```

Install the gem manually by running:

```bash
rake gem:install
```

in the application folder.

Author
------

Original author: Alfred Moreno

License
-------

(The MIT License)

Copyright (c) 2012 Alfred Moreno

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
