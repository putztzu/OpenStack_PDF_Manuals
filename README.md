OpenStack_PDF_Manuals
=================

PDFs generated from source on or about the day of the file date

To get latest, always generate from source, source can be downloaded
https://github.com/ajaeger/openstack-manuals.git

Follow instructions to use maven.
The README.md desribes yum and apt methods, if you are using openSUSE you can search http://software.opensuse.org for current or latest "maven" then use 1-click install.

With an Internet connection, and from within each branch which contains a pom.xml, execute the following
mvn clean generate sources

The following script builds the entire documentation after downloading source and installing maven (Will take approx 30 minutes, YMMV network connection and system processes)

cd <path to git root>openstack-manuals/doc/src/docbks/basic-install
mvn clean generate sources
cd ../cli-guide
mvn clean generate sources
cd ../openstack-block-storage-admin
mvn clean generate sources
cd ../openstack-compute-admin
mvn clean generate sources
cd ../openstack-ha
mvn clean generate sources
cd ../openstack-install
mvn clean generate sources
cd ../openstack-object-storage-admin
mvn clean generate sources
cd ../openstack-ops
mvn clean generate sources

Use information in this document at the User's own risk

