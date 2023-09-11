
# Host network mode
- Host network mode bypasses the Docker’s built-in virtual network and maps container ports directly to your EC2 
  instance’s network interface
- This mode shares the same network namespace of the host EC2 instance so your containers share the same IP with your 
  host IP address
- This also means that you can’t have multiple containers on the host using the same port
- A port used by one container on the host cannot be used by another container as this will cause conflict
- This mode offers faster performance than the bridge network mode since it uses the EC2 network stack instead of the 
  virtual Docker network