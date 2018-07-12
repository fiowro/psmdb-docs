.. _tarball:

=========================================================
Installing Percona Server for MongoDB from Binary Tarball
=========================================================

You can find links to the binary tarballs from the
`Percona Server for MongoDB download page <https://www.percona.com/downloads/percona-server-mongodb-3.4/>`_.

1. Fetch and extract the correct binary tarball.
   For example, if you are running Debian 8 ("jessie"):

   .. code-block:: bash

      wget https://www.percona.com/downloads/percona-server-mongodb-3.4/percona-server-mongodb-3.4.15-2.13/binary/debian/jessie/x86_64/percona-server-mongodb-3.4.15-2.13-r5b5e6df-jessie-x86_64-bundle.tar
      tar xfz percona-server-mongodb-3.4.15-2.13-r5b5e6df-jessie-x86_64-bundle.tar

2. Copy the extracted binaries to the target directory, for example:

   .. code-block:: bash

      mkdir ~/psmdb
      cp -r -n percona-server-mongodb-3.4.15-2.13-r5b5e6df-jessie-x86_64-bundle/bin ~/psmdb/

3. Add the location of the binaries to the ``PATH`` variable:

   .. code-block:: bash

      export PATH ~/psmdb/bin:$PATH

4. Create the default data directory:

   .. code-block:: bash

      mkdir -p /data/db

5. Make sure that you have read and write permissions for the data directory
   and run ``mongod``.

