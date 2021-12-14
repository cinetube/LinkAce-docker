# LinkAce-docker

```
git clone https://github.com/cinetube/LinkAce-docker/
```

```
cd LinkAce-docker
```


```
docker-compose up -d
```

After you started the Docker containers, you are almost ready to run the setup. Before the setup, we have to generate a secret key.

```
docker exec linkace-app-1 php artisan key:generate
```

If you are unsure if the .env file is writable inside Docker, please make it writable for anybody (-rw-rw-rw- or 666). You can switch back to make it read only after the setup.

```
chmod 666 .env
```

```
chmod 777 linkace_logs/
```
