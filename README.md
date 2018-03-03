# Build EJBCA Server From Scratch

Usage:
./ejbca-setup

Answer questions and get a running EJBCA@Wildfly10

# Set Up

Some parameters needed to be set in script.

## Required Settings

Set your hostname (visible in Internet), database etc.

httpsserver_hostname="ejbca.example.com"
database_host="mysql"
database_name="ejbca"
database_url="jdbc:mysql://${database_host}:3306/${database_name}?characterEncoding=UTF-8"
database_driver="org.mariadb.jdbc.Driver"
database_username="ejbca"
database_password="very***bad***database***password"

## Optional Settings

Change only if you know what you are doing

WILDFLY_VERSION="10.1.0.Final"
EJBCA_MAJOR_VERSION="ejbca6"
EJBCA_MINOR_VERSION="ejbca_6_10_0"
EJBCA_RELEASE="6_10_1_2"
MARIADB_CONNECTOR_VERSION="2.2.2"

## Set Up First Certificate/CA

superadmin_cn="SuperAdminDemo"
ca_name="ManagementCA"
BASE_DN="O=Example CA,C=DE"
ca_dn="CN=ManagementCA,${BASE_DN}"

