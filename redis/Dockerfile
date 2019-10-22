FROM redis:4
ENV REDIS_PASSWORD NkJBsgrUqPa2t4iFuMsRUZ8v
COPY ./redis.conf /usr/local/etc/redis/redis.conf
CMD ["sh", "-c", "exec redis-server  \/usr\/local\/etc\/redis\/redis.conf --requirepass \"$REDIS_PASSWORD\""]
