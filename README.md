python.org
==========

The new python.org!

Getting going
-------------

Requires :sparkles:Python 3.3!:sparkles: (`brew install python3`)

You'll want a virtualenv. Python 3.3 actually includes virtualenv built-in,
so you can do:

    $ pyvenv-3.3 <env>
    $ source <env>/bin/activate
    (etc)

But you can also use your existing virtualenv/wrapper:

    $ mkvirtualenv --python=python3.3 <env>

And then it's the standard:

    $ pip install -r requirements.txt
    $ ./manage.py syncdb

This expects a local database named "python.org". If you need to change it:

    $ export DATABASE_URL=postgres://user:pass@host:port/dbname

