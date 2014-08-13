# Database Assets

The file work-postgres.psql contains a prelimiary database dump of data collected. This data is currently a work in progress and the data is completely flat, string based and un-normalized.

The file saf-reports-postgres.psql contains database tables compiled from SAF XML reports. The data is currently a work in progress and the data is completely flat, string based and un-normalized.


#### Restoring the OOI Metadata Database

```
createdb ooimeta
pg_restore -d ooimeta work-postgres.psql
```

A bunch of warnings will be displayed concerning roles.

#### Restoring the OOI Metadata Database

```
createdb saf
pg_restore -d saf saf-reports-postgres.psql
```

A bunch of warnings will be displayed concerning roles.
