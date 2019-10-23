FROM nginx:1.13.3

RUN apt-get update && apt-get install -y --no-install-recommends htop procps

ADD ./nginx.conf /etc/nginx/nginx.conf

# Clear cache
RUN apt-get clean && rm -rf /var/lib/apt/lists/*