
# Bridge network mode – Default
- When you select the <default> network mode, you are selecting the Bridge network mode
- This is the default mode for Linux containers
- For Windows Docker containers, the <default> network mode is NAT
- Bridge network mode utilizes Docker’s built-in virtual network which runs inside each container
- A bridge network is an internal network namespace in the host that allows all containers connected on the same bridge 
  network to communicate
- It provides isolation from other containers not connected to that bridge network
- The Docker driver handles this isolation on the host machine so that containers on different bridge networks cannot 
  communicate with each other
- This mode can take advantage of dynamic host port mappings as it allows you to run the same port (ex: port 80) on each 
  container, and then map each container port to a different port on the host
- However, this mode does not provide the best networking performance because the bridge network is virtualized and 
  Docker software handles the traffic translations on traffic going in and out of the host
