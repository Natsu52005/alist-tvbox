# alist-tvbox
AList proxy server for TvBox, support playlist.

# Deploy
```bash
java -jar target/alist-tvbox-1.0.jar
```

# Docker
```bash
./build.sh
docker run -d -p 8080:8080 --restart=always --name=alist-tvbox alist-tvbox
```

# TvBox Config
```json
{"key":"Alist","name":"Alist┃转发","type":1,"api":"http://ip:8080/vod?site=http://alist:5244","searchable":2,"quickSearch":0,"filterable":0}
```
