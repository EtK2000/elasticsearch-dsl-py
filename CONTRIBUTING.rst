Contribution Guide
==================

If you have a bugfix or new feature that you would like to contribute to
elasticsearch-dsl-py, please find or open an issue about it first. Talk about what
you would like to do. It may be that somebody is already working on it, or that
there are particular issues that you should know about before implementing the
change.

If you want to be rewarded for your contributions, sign up for the
`Elastic Contributor Program <https://www.elastic.co/community/contributor>`_.
Each time you make a valid contribution, you’ll earn points that increase your
chances of winning prizes and being recognized as a top contributor.

We enjoy working with contributors to get their code accepted. There are many
approaches to fixing a problem and it is important to find the best approach
before writing too much code.

The process for contributing to any of the Elasticsearch repositories is similar.

1. Please make sure you have signed the `Contributor License
   Agreement <https://www.elastic.co/contributor-agreement/>`_. We are not
   asking you to assign copyright to us, but to give us the right to distribute
   your code without restriction. We ask this of all contributors in order to
   assure our users of the origin and continuing existence of the code. You only
   need to sign the CLA once.

2. Many classes included in this library are offered in two versions, for
   asynchronous and synchronous Python. When working with these classes, you only
   need to make changes to the asynchronous code, located in *_async*
   subdirectories in the source and tests trees. Once you've made your changes,
   run the following command to automatically generate the corresponding
   synchronous code:

    .. code:: bash

        $ nox -rs format
   
3. Run the test suite to ensure your changes do not break existing code:

    .. code:: bash

        $ nox -rs lint test

4. Rebase your changes.
   Update your local repository with the most recent code from the main
   elasticsearch-dsl-py repository, and rebase your branch on top of the latest master
   branch. We prefer your changes to be squashed into a single commit.

5. Submit a pull request. Push your local changes to your forked copy of the
   repository and submit a pull request. In the pull request, describe what your
   changes do and mention the number of the issue where discussion has taken
   place, eg “Closes #123″.  Please consider adding or modifying tests related to
   your changes. Include any generated files in the *_sync* subdirectory in your
   pull request.

Then sit back and wait. There will probably be discussion about the pull
request and, if any changes are needed, we would love to work with you to get
your pull request merged into elasticsearch-dsl-py.
