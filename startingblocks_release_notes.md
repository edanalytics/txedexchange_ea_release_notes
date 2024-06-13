# StartingBlocks Release Notes

StartingBlocks is a manged Ed-Fi hosting service. 

## dev-2023 environment
### initial deployment, 2023-07-11

- EdFi Suite 3, version 5.3
- Data standard, version 3.3.1-b
- TX Extensions, version 2023.2.2
- App code is built from MetaEd
- DB structure is built from MetaEd for PostgreSQL
- Environment is configured in District Specific mode
- ODS created for all 1280 LEAs
- Seed data and claimsets copied from TSDS SDK
- App infrastructure is Docker in Elastic Beanstalk
- DB infrastructure is Aurora PostgreSQL
- All data-flow paths are encrypted in transit and at rest

## dev-2024 environment
### initial deployment, 2023-07-12

- EdFi Suite 3, version 6.1
- Data standard, version 4.0.0
- TX Extensions, version 2024.1.0
- App code is pulled from TSDS SDK
- DB structure is built from MetaEd for PostgreSQL
- Environment is configured in District Specific mode
- ODS created for all 1280 LEAs
- Seed data and claimsets copied from TSDS SDK
- App infrastructure is Docker in Elastic Beanstalk
- DB infrastructure is Aurora PostgreSQL
- All data-flow paths are encrypted in transit and at rest

## integration-2024 environment
### initial deployment, 2023-07-26

- EdFi Suite 3, version 6.1
- Data standard, version 4.0.0
- TX Extensions, version 2024.1.0
- App code is pulled from TSDS SDK
- DB structure is built from MetaEd for PostgreSQL
- Environment is configured in District Specific mode
- ODS created for all 1280 LEAs
- Seed data and claimsets copied from TSDS SDK
- App infrastructure is Docker in Elastic Beanstalk
- DB infrastructure is Aurora PostgreSQL
- All data-flow paths are encrypted in transit and at rest


## preprod-2024-2-2 environment
### initial deployment, 2024-05-22

- EdFi Suite 3, version 7.1
- Data standard, version 4.0.0
- TX Extensions, version 2024.2.2
- App code is pulled from TSDS SDK
- DB structure is built from MetaEd for PostgreSQL
- Environment is configured in multitenant mode
    - `preprod` tenant created
        - ODS created for all 1280 LEAs
    - `dev` tenant created
        - ODS will be created as necessary
- Seed data and claimsets copied from TSDS SDK
- App infrastructure is Docker in Elastic Beanstalk
- DB infrastructure is Aurora PostgreSQL
- All data-flow paths are encrypted in transit and at rest


