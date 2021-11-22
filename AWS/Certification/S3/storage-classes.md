# Storage Classes

## S3 Standard
High Availability and Durability.

Stored reduntantly across multiple devices in multiple facilities ( >=3 AZs).

99.99% Availability

99.99999999999 Durability (11 9's) - not getting corupted or lost
Designed for frequent access

Suitable for:
- websites
- content distribution, mobile and gaming apps
- big data analytics

## S3 Standard-Infrequent Access (S3-IA)
- Accessed less frequently
- Radid access when needed
- pay to access - low perGB storage price and perGB reteival
- minimum storage time 30 days

Good for:
- long term storage, backups

99.99% Availability

99.99999999999 Durability (11 9's) - not getting corupted or lost

## S3 One Zone-Infrequent Access
like above but a single AZ only

20% less that regular S3-IA

Good for infrequently accessed non critical data

Difference:

95.99% Availability


## S3 Glacier and S3 Glacier Deep Archive
- Cheap storage
- very infrequent use
- minimum storage time is 90 days
- Stored reduntantly across multiple devices in multiple facilities ( >=3 AZs). 
- 99.99% Availability
- 99.99999999999 Durability (11 9's) - not getting corrupted or lost

### Glacier deep archive
As above except:
- minimum storage time is 180 days
- 12 hour retrieval time

Used for compliance records



## Intelligent-Tiering