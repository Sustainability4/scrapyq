# ScrapyDocker

### Project goal - 
Create an async API which queues (and executes) scraping requests for input scrapy spider and url

1. Expose scrapy project to an endpoint using scrapyrt - ![#c5f015](https://via.placeholder.com/15/c5f015/c5f015.png) Complete
2. Create an external handler to handle scraping requests - ![#c5f015](https://via.placeholder.com/15/c5f015/c5f015.png) Complete
3. Queue async requests using redis and rq - ![#c5f015](https://via.placeholder.com/15/c5f015/c5f015.png) Complete
4. Replace rq with Celery - ![#f03c15](https://via.placeholder.com/15/f03c15/f03c15.png) Pending
5. Add mongodb backend to dump outputs - ![#f03c15](https://via.placeholder.com/15/f03c15/f03c15.png) Pending
6. Add scheduler using celery - ![#f03c15](https://via.placeholder.com/15/f03c15/f03c15.png) Pending

### Docker Stack: 
scrapy, scrapyrt, flask, redis, rq


### To build and run docker containers:
```
cd scrapyrt_docker
docker-compose build --no-cache
docker-compose up
```

To test API, import the POSTMAN collection `utils/postman_collection.json`