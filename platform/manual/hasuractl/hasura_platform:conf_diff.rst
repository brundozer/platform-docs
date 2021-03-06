.. _hasura_platform:conf_diff:

Hasura CLI: hasura platform:conf diff
-------------------------------------

Diff configuration of clusters

Synopsis
~~~~~~~~


Diff configuration of two clusters, if second cluster is not provided, diff is shown against the server config

::

  hasura platform:conf diff [flags]

Examples
~~~~~~~~

::

    # Show diff of the local config for a cluster called 'staging' with its server:
    $ hasura conf diff -c staging
    # Show diff of a cluster called 'staging' against another cluster called 'production':
    $ hasura conf diff -c staging -c production

Options
~~~~~~~

::

  -c, --cluster stringArray   clusters on which diff has to be run. If only one cluster is given, it's applied and local versions are diffed
  -h, --help                  help for diff

Options inherited from parent commands
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

::

      --project string   hasura project directory where the commands should be executed. (default: current directory)

SEE ALSO
~~~~~~~~

* :ref:`hasura platform:conf <hasura_platform:conf>` 	 - Manage configuration on the cluster

*Auto generated by spf13/cobra*
