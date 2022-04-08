# ww-dta-mpexp

This data export format is available for products ImmoTop, ImmoTop2, Rimo R4 and Rimo R5.
The dataset is designed to provide realestate status information to a third party system.

## Overview

The data is deliverd in a flat structured CSV-file.

- realestate
- unit
- tenant/condominium owner
- property manager
- facility manager
- registration code

## Export & Data Transfer

The process of exporting and transfering the datefile is set up ERP specific an depends on licenced tools and releaseversion in customer environment.
Depending on software, releaseversion, environment, licenced tools the data export has to be done manually by user or could set up completely automatic.
For further questions customer should contact w&w directly.

## Licence

This data export format is an optional module to be licenced by the customer.
For further questions customer should contact w&w directly.

## Export Format

Filename: indidually configurable
Format: CSV
Delimiter: ;

Some columns might not be provided depending on "export type" defined in ERP system

| column                   | m   | id  | example                                       | remarks                                                             |
| ------------------------ | --- | --- | --------------------------------------------- | ------------------------------------------------------------------- |
| customer_id              | x   | x   | X0135816FZHK                                  | unique customer identifier                                          |
| property_id              | x   | x   | 10001                                         |
| property_name            | x   |     | Löwenstrasse 1-7                              |
| group_id                 | x   | x   | 1                                             |
| group_name               | x   |     | Löwenstrasse 1                                |
| unit_adress_street_name  |     |     | Löwenstrasse 1                                |
| unit_adress_postcode     |     |     | 8910                                          |
| unit_adress_city         |     |     | Affoltern am Albis                            |
| unit_adress_country      |     |     | 756                                           | country code numeric: https://www.iso.org/obp/ui/#search            |
| unit_id                  | x   | x   | 11101                                         |
| unit_name                |     |     | 3.5 Zimmerwohnung 1. OG links                 |
| unit_type                |     |     | Wohnung                                       |
| unit_square_meter        |     |     | 80                                            | area in m2                                                          |
| unit_level               |     |     | 1                                             | 0-EG,1-1.St,2-2.St,3-3.St,…,99-Dach,-1-1.UG,-2-2.UG,-3-3.UG,...     |
| utilisation_period_start | x   | x   | lease start                                   |
| utilisation_period_end   |     |     | lease end                                     |
| contract_type            | x   |     | 1                                             | 1 = tenancy, 2 = condominum ownership                               |
| user1_id                 |     |     | 560                                           | **unique person id for user 1**                                     |
| user1_name               |     |     | Hans Muster                                   | exporttypes 1/2: name & prename or companyname, exporttype 3 = name |
| user1_prename            |     |     | Hans                                          | exporttype 3                                                        |
| user1_companyname        |     |     | W&W Immo Informatik AG                        | exporttype 3                                                        |
| user1_email              |     |     | test@wwimmo.ch                                |                                                                     |
| user1_phone1             |     |     | 012 345 67 89                                 |                                                                     |
| user1_phone2             |     |     | 012 345 67 89                                 |                                                                     |
| user1_adress             |     |     | Löwenstrasse 1 &#124; 8910 Affoltern am Albis | exporttypes 1/2                                                     |
| user1_adress_street_name |     |     | Löwenstrasse 1                                | exporttype 3                                                        |
| user1_adress_postcode    |     |     | 8910                                          | exporttype 3                                                        |
| user1_adress_city        |     |     | Affoltern am Albis                            | exporttype 3                                                        |
| user1_adress_country     |     |     | 756                                           | country code numeric: https://www.iso.org/obp/ui/#search            |
| user2_id                 |     |     | 562                                           | **unique person id for user 2**                                     |
| user2_name               |     |     | Hans Muster                                   | exporttypes 1/2: name & prename or companyname, exporttype 3 = name |
| user2_prename            |     |     | Hans                                          | exporttype 3                                                        |
| user2_companyname        |     |     | W&W Immo Informatik AG                        | exporttype 3                                                        |
| user2_email              |     |     | test@wwimmo.ch                                |                                                                     |
| user2_phone1             |     |     | 012 345 67 89                                 |                                                                     |
| user2_phone2             |     |     | 012 345 67 89                                 |                                                                     |
| user2_adress             |     |     | Löwenstrasse 1 &#124; 8910 Affoltern am Albis | exporttypes 1/2                                                     |
| user2_adress_street_name |     |     | Löwenstrasse 1                                | exporttype 3                                                        |
| user2_adress_postcode    |     |     | 8910                                          | exporttype 3                                                        |
| user2_adress_city        |     |     | Affoltern am Albis                            | exporttype 3                                                        |
| user2_adress_country     |     |     | 756                                           | country code numeric: https://www.iso.org/obp/ui/#search            |
| user3_id                 |     |     | 563                                           | **unique person id for user 3**                                     |
| user3_name               |     |     | Hans Muster                                   | exporttypes 1/2: name & prename or companyname, exporttype 3 = name |
| user3_prename            |     |     | Hans                                          | exporttype 3                                                        |
| user3_companyname        |     |     | W&W Immo Informatik AG                        | exporttype 3                                                        |
| user3_email              |     |     | test@wwimmo.ch                                |                                                                     |
| user3_phone1             |     |     | 012 345 67 89                                 |                                                                     |
| user3_phone2             |     |     | 012 345 67 89                                 |                                                                     |
| user3_adress             |     |     | Löwenstrasse 1 &#124; 8910 Affoltern am Albis | exporttypes 1/2                                                     |
| user3_adress_street_name |     |     | Löwenstrasse 1                                | exporttype 3                                                        |
| user3_adress_postcode    |     |     | 8910                                          | exporttype 3                                                        |
| user3_adress_city        |     |     | Affoltern am Albis                            | exporttype 3                                                        |
| user3_adress_country     |     |     | 756                                           | country code numeric: https://www.iso.org/obp/ui/#search            |
| user4_id                 |     |     | 564                                           | **unique person id for user 4**                                     |
| user4_name               |     |     | Hans Muster                                   | exporttypes 1/2: name & prename or companyname, exporttype 3 = name |
| user4_prename            |     |     | Hans                                          | exporttype 3                                                        |
| user4_companyname        |     |     | W&W Immo Informatik AG                        | exporttype 3                                                        |
| user4_email              |     |     | test@wwimmo.ch                                |                                                                     |
| user4_phone1             |     |     | 012 345 67 89                                 |                                                                     |
| user4_phone2             |     |     | 012 345 67 89                                 |                                                                     |
| user4_adress             |     |     | Löwenstrasse 1 &#124; 8910 Affoltern am Albis | exporttypes 1/2                                                     |
| user4_adress_street_name |     |     | Löwenstrasse 1                                | exporttype 3                                                        |
| user4_adress_postcode    |     |     | 8910                                          | exporttype 3                                                        |
| user4_adress_city        |     |     | Affoltern am Albis                            | exporttype 3                                                        |
| user4_adress_country     |     |     | 756                                           | country code numeric: https://www.iso.org/obp/ui/#search            |
| property_manager1_name   |     |     | Hans Property                                 | name & prename                                                      |
| property_manager1_email  |     |     | hp@immo.ch                                    |
| property_manager1_phone1 |     |     | 098 765 43 21                                 |
| property_manager1_phone2 |     |     |                                               |
| property_manager2_name   |     |     |                                               | name & prename                                                      |
| property_manager2_email  |     |     |                                               |
| property_manager2_phone1 |     |     |                                               |
| property_manager2_phone2 |     |     |                                               |
| facility_manager_name    |     |     | Maria Rito                                    | name & prename                                                      |
| facility_manager_email   |     |     | maria.rito@facility.ch                        |
| facility_manager_phone1  |     |     |                                               |
| facility_manager_phone2  |     |     |                                               |
| timestamp_export         |     |     | 18.03.2022                                    | export date                                                         |
| registration_code1       |     |     |                                               | exporttype 1: code could be used to sign up user 1                  |
| registration_code2       |     |     |                                               | exporttype 1: code could be used to sign up user 2                  |
| registration_code3       |     |     |                                               | exporttype 1: ode could be used to sign up user 3                   |
| registration_code4       |     |     |                                               | exporttype 1: code could be used to sign up user 4                  |

_column "m" = mandatory, this column has always a value. column "id" = unique identifier of a tenancy/condominium ownership_

## export types

1 - with registration codes but without explicit user data
2 - with user data in combined fields
3 - with user data in seperate fields
