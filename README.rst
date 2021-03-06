===============================
rehabstudio QA Docs
===============================


This repository provides (or will provide, once it's a bt more complete) a
central platform to host all our QA guidelines and agreed coding
standards for our entire stack.

These docs are hosted on Read The Docs at: http://qadocs.rehabstudio.com


Prerequisites
-------------

In order to build and use this documentation locally you'll need a standard Python 2.7 environment set up with `virtualenv` (and ideally `virtualenvwrapper`) installed. Installing and using those tools is outside the scope of this guide, but you can find detailed guides for your platform at http://docs.python-guide.org.

For ubuntu this is as simple as `sudo apt-get install python-dev virtualenvwrapper`, other platforms may differ.

Simple instructions on the usage of virtualenvwrapper can be found at http://docs.python-guide.org/en/latest/dev/virtualenvs/#id3.


Contributing
------------

Contributions are welcome, and they are greatly appreciated! Every
little bit helps, and credit will always be given.

Ready to contribute? Here's how to set up `rehabstudio/qadocs` for local
development.

1. Fork the `rehabstudio/qadocs` repo on GitHub.

2. Clone your fork locally::

    $ git clone git@github.com:your_name_here/qadocs.git
    $ cd qadocs/

3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development (Note that you should not need to use `sudo` at this point)::

    $ mkvirtualenv qadocs
    $ pip install -r requirements.txt

4. Create a branch for local development::

    $ git checkout -b name-of-your-bugfix-or-feature

   Now you can make your changes locally.

5. Build your new changes to test locally::

    $ make html

   Or if you prefer, run the included `watch.sh` script to continually monitor your repo for changes and rebuild as required::

    $ ./watch.sh

6. You can run a simple HTTP server locally (probably in another terminal) to view your changes::

    $ cd build/html && python -m SimpleHTTPServer

7. Commit your changes and push your branch to GitHub::

    $ git add .
    $ git commit -m "Your detailed description of your changes."
    $ git push origin name-of-your-bugfix-or-feature

8. Submit a pull request through the GitHub website.
