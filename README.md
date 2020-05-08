# ttrss-opencc
Conversion between Traditional and Simplified Chinese via OpenCC for ttrss

## Deploy your own OpenCC API Server

```
docker run -d -p 3000:3000 wangqiru/opencc_api_server
```

Alternatively, deploy this all-in-one TTRSS docker: [HenryQW/docker-ttrss-plugins](https://github.com/HenryQW/docker-ttrss-plugins)

```
docker run -it --name ttrss --restart=always \
-e SELF_URL_PATH = [ your URL ]  \
-e DB_HOST = [ your DB address ]  \
-e DB_PORT= [ your DB port ]  \
-e DB_NAME = [ your DB name ]  \
-e DB_USER = [ your DB user ]  \
-e DB_PASS = [ your DB password ]  \
-p [ your port ]:80  \
-d wangqiru/ttrss
```
