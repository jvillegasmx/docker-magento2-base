# docker-magento2-base
Docker installation  for magento2, you can use it to install Magento 2.1.6


Rename .project-env.demo to .project-env with your custom params

The public files are in the folder "pub", you can use it to install magento 2.x
After building all just go to http:127.0.0.1 and you can see the files.

for run

docker-compose up -d //will  run and build the containers
docker ps //to check the IDs containers.
docker exec -ti CONTAINER_ID /bin/bash //Access to the container

docker inspect magento_iedux_database //to check the details Host IP of the database docker


Reindex Magento
/usr/bin/php /var/www/html/bin/magento  indexer:reindex
