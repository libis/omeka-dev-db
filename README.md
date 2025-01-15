You can access the phpMyAdmin at http://localhost:8090/

MYSQL is available on port 3308

To use command line mysql:
 docker exec -it db mysql -u root -p 

Use 'db' as hostname in database.ini files 

Add the following to a seperate project's docker-compose.yml:
    services:
      ...
      networks:
       - my-network
      ...

    networks:
      my-network:
        external:
          name: dev-network

