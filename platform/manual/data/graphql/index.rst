=================
GraphQL on Hasura
=================

Starting from version ``v0.15.31``, the data microservice supports querying over `GraphQL <https://graphql.org/>`_
in addition to the JSON based query language. The ``API Explorer`` section of the :doc:`API console <../../api-console/index>`
has `GraphiQL <https://github.com/graphql/graphiql>`_ integrated to let you explore the GraphQL APIs of Hasura.

Quick overview
--------------

1. Getting GraphQL APIs over a table:

   - :ref:`Create a table <data-create-tables>`.
   - That's it. The GraphQL APIs are ready. You can try them out at the :ref:`API Explorer <api_explorer>`.

2. Adding another table to GraphQL schema:

   - Create another table just like you did in *1*.
   - Another table has been added to the schema :-)

3. Linking the two tables and getting GraphQL APIs over them:

   - :ref:`Create a relationship <data-create-relationships>` between the two tables.
   - GraphQL APIs over the relationship are ready. You can start :ref:`fetching <data-fetching-relationships>` over them.

4. Access control for your tables:

   - Set :ref:`permissions <data-permissions>` over your tables.
   - Once you set permissions, the GraphQL queries and mutations will respect these permissions.

To know about the GraphQL API in detail, check out the :ref:`reference <data-graphql>`.

.. admonition:: Note

    If you already have a Postgres database and wish to have GraphQL APIs over it, we have a quick guide for migrating
    your database :ref:`here <guide-import-existing-database>`.

See:
^^^^

.. toctree::
  :maxdepth: 1

    GraphQL Schema <schema>
    Custom Resolvers using Views <customise-schema-views>
    Write your own resolver <write-your-own-resolvers>
    Schema Stitching <schema-stitching>
    Reference <reference>
