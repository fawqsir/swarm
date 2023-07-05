#Create a traefik network dhcp range will be 172.20.1.0/24 while static ips can be reached 172.20.0.0/24
docker network create --driver=overlay --ip-range 172.20.1.0/24 --subnet 172.20.0.0/22 --gateway 172.20.0.1 traefik-public
