
Contributing
============

gmaps is a very new project, so there is a lot of scope for developpers to make
a strong impact by contributing code, documentation and expertise. All
contributions are welcome.

How to contribute
-----------------

The `documentation <http://docs.scipy.org/doc/numpy/dev/gitwash/index.html>`_ for Numpy gives a detailed description of how to contribute. Most of this information applies to development for ``gmaps``.

Developping with git
^^^^^^^^^^^^^^^^^^^^

You will need the `Git version control system <http://git-scm.com>`_ and an account on `Github <https://github.com>`_ to
contribute to gmaps.

1. Fork the `project repository <http://github.com/pbugnion/gmaps>`_ by clicking `Fork` in the top right of the page. This will create a copy of the fork under your account on Github.

2. Clone the repository to your computer::
   
    $ git clone https://github.com/YourUserID/gmaps.git

3. Install gmaps by running::

    $ pip install -e "."

   in the package's root directory. 


You can now make changes and contribute them back to the source code:

1. Create a branch to hold your changes::

    $ git checkout -b my-feature

   and start making changes.

2. Work on your local copy. When you are satisfied with the changes, commit
   them to your local repository::

    $ git add 'FILES THAT YOU MODIFIED'
    $ git commit

   You will be asked to write a commit message. Explain the reasoning behind
   the changes that you made.

3. Propagate the changes back to your github account::

    $ git push -u origin my-feature

4. To integrate the changes into the main code repository, click `Pull Request`
   on the `gmaps` repository page on your accont. This will notify the
   committers who will review your code.

Updating your repository
^^^^^^^^^^^^^^^^^^^^^^^^

To keep your private repository updated, you should add the main repository as 
a remote::
    
    $ git remote add upstream git://github.com/pbugnion/gmaps.git

To update your private repository, you can then fetch new commits from
upstream::

    $ git fetch upstream
    $ git rebase upstream/master


Guidelines
----------

Workflow
^^^^^^^^

We loosely follow the `git workflow <http://docs.scipy.org/doc/numpy/dev/gitwash/development_workflow.html>`_ used in numpy development.  Features should
be developped in separate branches and merged into the master branch when
complete. Avoid putting new commits directly in your ``master`` branch.


Code
^^^^

Please follow the `PEP8 conventions <http://www.python.org/dev/peps/pep-0008/>`_ for formatting and indenting code and for variable names.
