### Intro
Docker environment for Fanshawe Lab Shenanigans


#### Set up
1. Clone the repo
   ```
   git clone git@github.com:spiderPan/fanshawe_lab_shenanigans.git
   ```
2. Open the folder and run docker-compose up
   ```
   cd fanshawe_lab_shenanigans
   docker-compose up
   ```


#### Comman URLs
1. Web server is in `http://localhost:8888` --> `./html/`
2. phpMyAdmin is in `http://localhost:8123`


#### Usage Notes

1. When connecting db, here is the info, please see the index.php under html for usage example

| Attribute     | Value   |   |   |   |   |   |
|---------------|---------|---|---|---|---|---|
| Host          | mysql   |   |   |   |   |   |
| Username      | test_u  |   |   |   |   |   |
| Password      | test_p  |   |   |   |   |   |
| Database Name | db_test |   |   |   |   |   |


2. Currently PHP is 7.3 within apache, with `mysqli`, `pdo` and `json` PHP extension enabled. If you need other extensions, please reach out Pan.

3. Init DB can automatically imported from `./.docker/data`, simply put any `.sql` file within the folder and it will imported into `db_test` when first time run `docker-compose up`. By all means, you can always manage it through phpMyAdmin later.