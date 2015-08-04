Multi Cloud Command Line API

This is a command line client and API for implementing various services in multiple Openstack cloud/regions. Currently one service has been implemented i.e creating tenants in multiple clouds simultaneously.

INSTALLATION:

This package can be installed using pip:

sudo pip install git+https://gecgithub01.walmart.com/rnagpal/python-multicloudclient.git

REQUIREMENTS:

For multi tenant services , the environment variables are specific to the regions in which multitenant needs to be created. So for every region following environment variables needs to be created.

export OS_USERNAME_=

export OS_PASSWORD_=

export OS_TENANT_NAME_=

export OS_AUTH_URL_=

For example for region 1 R1:

export OS_USERNAME_R1=

export OS_PASSWORD_R1=

export OS_TENANT_NAME_R1=

export OS_AUTH_URL_R1=

COMMAND LINE ARGUMENT FOR CREATING TENANTS ACROSS MULTIPLE CLOUDS:

multi-cloud create-tenants --tenant_id multi --owner rajat --email rajat.nagpal@sjsu.edu --regions R1,R2

The details for the command are:

usage: multi-cloud create-tenants [--tenant_id (tenant-id)] [--owner (user)] [--email (email-id)] [--regions (comma separated regions)]

create-tenants: service for creating multiple tenants
