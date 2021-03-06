## Typical Docker Commands
    ### Start all environments services
    > docker-compose up --build
    
    ### Restart a specific container
    > docker restart [service name]
    
    ### List all containers
    > docker ps -a
    
    ### List running containers
    > docker ps
    
    ### See used space
    > docker system df
    
    ### Remove un-used data
    > docker system prune

## Passwords
    ### PostgreSQL
    > username: postgres_user
    > password: postgres_pass
    
    ### MySql
    > username: mysql_user
    > password: mysql_pass
    
    ### MariaDB
    > username: mariadb_user
    > password: mariadb_pass


## Running Xdebug with PHPStorm alongside Docker.
Any logic that needs to speak to the host machine will need to point to the IP of `10.254.254.254`.

For Xdebug to work through PHPStorm first execute:

```
sudo ifconfig lo0 alias 10.254.254.254
```