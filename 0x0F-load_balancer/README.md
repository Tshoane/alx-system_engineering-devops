[200~
Project 0x0B: Web Server Configuration Expansion
Introduction
In this project, the objective is to scale up the web server configuration by doubling the number of web servers and implementing a load balancer to manage them effectively. Two additional servers will be added, one to replicate the Nginx configuration of the original server, and another to set up an HAproxy load balancer.

Tasks Overview
0. Double the number of webservers
Script Name: 0-custom_http_response_header

This Bash script installs and configures Nginx on a server with a custom HTTP response header.

The custom HTTP header is named X-Served-By.
The value of the HTTP header is the hostname of the server.
1. Install your load balancer
Script Name: 1-install_load_balancer

This Bash script installs and configures HAproxy version 1.5 on a server.

Enables management via the init script.
Requests are distributed using a round-robin algorithm.
2. Puppet custom HTTP response header
Script Name: 2-puppet_custom_http_response_header.pp

This script automates the task of creating a custom HTTP header response using Puppet.

The custom HTTP header's name is X-Served-By.
The value of the custom HTTP header is the hostname of the server Nginx is running on.
Conclusion
Expanding the web server configuration involves doubling the number of servers and setting up a load balancer to efficiently manage incoming requests. By following the specified tasks, the infrastructure can be scaled up while ensuring proper distribution of traffic across the web servers.
