ps -ef | grep -i 'redis-server'
sudo nano /etc/redis/redis.conf
    bind 127.0.0.1 ::1   ->   bind 127.0.0.1   ->   bind 127.0.0.1 ::1

sudo kill -9 <PID>

celery worker -A image_parroter --loglevel=info