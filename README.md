# docker-for-typo3-v9

## Usefull commands 

Build/run containers with (with and without detached mode)

```bash
$ docker-compose build
$ docker-compose up -d
```

```bash
# bash commands
$ docker-compose exec php bash
```

## Initalisation of TYPO3 

```bash
php vendor/bin/typo3cms install:setup \
    --non-interactive \
    --database-user-name=user \
    --database-user-password=userpass \
    --database-host-name=db \
    --database-port=3306 \
    --database-name=mydb \
    --use-existing-database \
    --admin-user-name=admin \
    --admin-password=password \
    --site-setup-type=site
```

### Based on maxpou Docker files