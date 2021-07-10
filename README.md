# cockroachdb-movr

# First step

```shell
CREATE DATABASE movr;
USE movr;
```

```shell
CREATE TABLE vehicles (
        id UUID PRIMARY KEY,
        last_longitude FLOAT8,
        last_latitude FLOAT8,
        battery INT8,
        last_checkin TIMESTAMP,
        in_use BOOL,
        vehicle_type STRING NOT NULL
    );
```

```shell**
INSERT INTO vehicles (id, last_longitude, last_latitude, battery, last_checkin, in_use, vehicle_type) VALUES
	('0001b16c-36b9-4b3f-a2ff-566061f36e03', (-73.91734), 40.61334, 89, '2020-04-30 12:59:15+00:00', false, 'scooter'),
	('00077691-3be2-4440-a34c-f604c9716f99', (-74.42406), 40.70211, 40, '2020-04-30 00:11:08+00:00', false, 'scooter');
```