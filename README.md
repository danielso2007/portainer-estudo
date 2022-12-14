# Docker Portainer.io

[https://www.portainer.io/](https://www.portainer.io/)

# start.sh

Iniciar o container.

# stop.sh

Parar o container.

# down.sh

Para e remove tudo desse docker-compose (container e volumes).

# Acessando Portainer

[https://localhost:9443](https://localhost:9443)

# Gerando senha de admin para o container

`docker run --rm httpd:2.4-alpine htpasswd -nbB admin 'superpassword' | cut -d ":" -f 2`

A senha será `superpassword`.

Você precisa escapar cada `$` caractere dentro da senha com hash com outro `$`, exemplo:

`$2y$05$w5wsvlEDXxPjh2GGfkoe9.At0zj8r7DeafAkXXeubs0JnmxLjyw/a`

`$$2y$$05$$UhzeB20RRGl5MLL2cglmr.IvMkQ9zW41.OzdMX47g0NSRDc0zEZVe`