# Check Point CloudGuard AppSec demo
 
 This is a simple docker-compose environment for deploy a Check Point AppSec embedded nano-agent demo.  
 It will deploy three containers, an NGINX reverse proxy, an agent-container (the nano-agent) and the OWASP JuiceShop app.  

You will have two ways to access the stack:  
* Port 80: Protected by AppSec  
* Port 3000: Direct to JuiceShop (unprotected)  
  
## Instructions:
 
* Clone the repository
* From a machine with docker and docker-compose installed, run:  
`  export TOKEN=<your agent token>`  
`  docker-compose up `  
__Insert awesome demo here :)__  
`  docker-compose down `  
 


> Notes: 

> The NGINX config requires you to provide a host header otherwise you'll get a 404. The host header (eg, entry in your host file) should be *juiceshop.local*
> There are two ways to run docker compose: `docker-compose` and `docker compose`. Using `docker compose` (with a space, not a hyphen) is 'experimental' from a Docker perspective and seems to decide on its own value for IPC configuration and breaks this setup. Use `docker-compose` please :).
