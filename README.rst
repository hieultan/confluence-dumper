==============
How to install
==============
***************************
Configure virtualenv
***************************
For convenience you should use `virtualenvwrapper <http://virtualenvwrapper.readthedocs.io/en/latest/>`_::

 sudo pip install virtualenv

Create a new virtual environment::

    python3 -m venv venv

Enter the virtual environment::

    . venv/bin/activate

***************************
Configure confluence dumper
***************************
Install dependencies::

 pip install -r requirements.txt

Copy confluence settings::

 cd confluence_dumper
 cp settings.sample.py settings.py

Please personalize the ``settings.py`` on your own according to your confluence instance.

==========
How to use
==========
Don't forget to switch to the virtual environment because of the installed dependencies::

 . venv/bin/activate

Run confluence dumper::

 cd confluence_dumper
 python confluence_dumper.py
