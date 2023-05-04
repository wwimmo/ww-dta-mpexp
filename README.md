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
- owner
- registration code

## Export & Data Transfer

The process of exporting and transfering the datefile is set up ERP specific an depends on licenced tools and releaseversion in customer environment.
Depending on software, releaseversion, environment, licenced tools the data export has to be done manually by user or could set up completely automatic.
For further questions customer should contact w&w directly.

## Licence

This data export format is an optional module to be licenced by the customer.
For further questions customer should contact w&w directly.

## Export Format

[export-format](/export-format.md)

[example-file](/dta-mpexp.csv)

## Export Types

1 - with registration codes but without explicit user data<br>
2 - with user data in combined fields<br>
3 - with user data in seperate fields<br>

## Registration Code

With export type 1 each user entry gets a registration code (unique per customer and user).
The registration code has to be secure enough, so it's not possible for anyone to derive a code from a different user.

e.g. user registration code as uuid: 12a48666-651b-4809-87b9-535f5d40d9e5
