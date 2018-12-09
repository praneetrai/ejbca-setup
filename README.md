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
    database_username="ejbca"
    database_password="very***bad***database***password"

Double check these parameters. Really *all* parameters must
match your database, otherwise EJBCA will not run.

## Optional Settings

Change only if you know what you are doing

    WILDFLY_VERSION="10.1.0.Final"
    EJBCA_MAJOR_VERSION="ejbca6"
    EJBCA_MINOR_VERSION="ejbca_6_10_0"
    EJBCA_RELEASE="6_10_1_2"

## Set Up First Certificate/CA

    superadmin_cn="SuperAdminDemo"
    ca_name="ManagementCA"
    BASE_DN="O=Example CA,C=DE"
    ca_dn="CN=ManagementCA,${BASE_DN}"

