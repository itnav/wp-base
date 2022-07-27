# wp-base
## 初期起動
```
docker-compose up
```

## 起動後DBの設定変更(/wp/wp-config.php)
### Database username変更
```
define( 'DB_USER', getenv_docker('WORDPRESS_DB_USER', 'example username') );
```
'example username'→'wordpress'に変更

### Database password変更
```
define( 'DB_PASSWORD', getenv_docker('WORDPRESS_DB_PASSWORD', 'example password') );
```
'example password'→'wordpress'に変更
