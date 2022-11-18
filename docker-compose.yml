services:

  laravel-docker:
    container_name: laravel-docker
    build: .
    volumes:
      - ./laravel-app:/var/www/html
    ports:
      - 9000:80
  
  mysql_db:
    image: mysql:latest
    environment:
      MYSQL_ROOT_PASSWORD: root
      MYSQL_DATABASE: taravel_docker
    ports:
    - 3306:3306
  
  phpmyadmin:
    image: phpmyadmin:latest
    ports:
      - 9001:80
    environment:
      - PMA_ARBITRARY=1