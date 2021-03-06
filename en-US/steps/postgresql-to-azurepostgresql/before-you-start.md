## Preparing for database migration

As you prepare for migrating your database to the cloud, verify that your source environment is supported and that you have addressed any prerequisites. This will help to ensure an efficient and successful migration.

## Overview

This scenario describes how to migrate a PostgreSQL instance to Azure Database for PostgreSQL.

## Offline versus online migrations

For selected migration scenarios, Azure Database Migration Service supports both offline and online migrations. With an offline migration, application downtime begins when the migration starts. For an online migration, downtime is limited to the time required to cut over to the new environment when the migration completes.

**Important**: With PostgreSQL to Azure Database for PostgreSQL migrations, Azure Database Migration Service supports online migrations only.

## Supported versions

This section describes all supported scenarios and options for an upgrade from on-premises PostgreSQL versions to Azure Database for PostgreSQL. This information is current as of October 2019.

Details for migrations to Azure Database for PostgreSQL from the following PostgreSQL sources are included:

* PostgreSQL 9.5
* PostgreSQL 9.6
* PostgreSQL 10
* PostgreSQL 11

You can migrate PostgreSQL running on-premises or on AWS RDS.

## Overview of prerequisites

Before beginning your migration project, it is important to address the associated prerequisites for leveraging Azure Database Migration Service (DMS) for migrations. When upgrading from PostgreSQL to Azure Database for PostgreSQL, there are prerequisites associated with:

* Creating an instance of Azure Database for PostgreSQL (detail [here](https://docs.microsoft.com/azure/postgresql/quickstart-create-server-database-portal))
* Creating an instance of Azure Database Migration Service (detail [here](https://docs.microsoft.com/azure/dms/pre-reqs)).
* Using Azure Database Migration Service to perform online migrations from:
  * PostgreSQL (detail [here](https://docs.microsoft.com/azure/dms/tutorial-postgresql-azure-postgresql-online#prerequisites)).
  * RDS PostgreSQL (detail [here](https://docs.microsoft.com/azure/dms/tutorial-rds-postgresql-server-azure-db-for-postgresql-online#prerequisites)).

## Additional resources

* For a matrix of the Microsoft and third-party services and tools that are available to assist you with various database and data migration scenarios as well as specialty tasks, see the article [Service and tools for data migration](https://docs.microsoft.com/azure/dms/dms-tools-matrix).
* For an overview of the Azure Database Migration Guide and the information it contains, see the video [How to Use the Database Migration Guide](https://azure.microsoft.com/resources/videos/how-to-use-the-azure-database-migration-guide/).
* For a walk through of the phases of the migration process and detail about the specific tools and services recommended to perform assessment and migration, see the video [Overview of the migration journey and the tools/services recommended for performing assessment and migration](https://azure.microsoft.com/resources/videos/overview-of-migration-and-recommended-tools-services/).
* For a demo of how to migrate a PostgreSQL database running in an on-premises virtual machine to Azure Database for PostgreSQL with minimum downtime using the Azure CLI, see the video [How to migrate PostgreSQL to Azure Database for PostgreSQL with minimum downtime using DMS and the Azure CLI](https://azure.microsoft.com/resources/videos/how-to-migrate-postgresql-to-azure-postgresql-online-dms-and-cli/).
* For a walk through of the detailed workflow and a demo that shows how to migrate your application using minimal downtime to Azure Database for PostgreSQL, see the video [Migrate your PostgreSQL applications to Azure with minimal downtime using the Azure Database Migration Service](https://azure.microsoft.com/resources/videos/postg-migrate-vid/).
