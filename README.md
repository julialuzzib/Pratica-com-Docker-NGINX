# Prática-com-Docker-NGINX

## Cenário 1 — Startup de Delivery
A FastBite é uma startup de delivery de comida saudável fundada por dois amigos em Florianópolis. Nos primeiros meses, eles serviam o site diretamente de um servidor Node.js na porta 3000. Com o crescimento, o CTO percebeu que era insustentável: qualquer deploy derrubava o site, não havia separação de ambientes e o servidor ficava exposto diretamente na internet.

Você foi contratado como dev DevOps júnior. Sua primeira missão: containerizar a aplicação com Docker e colocar o Nginx como reverse proxy na frente, garantindo que o site responda na porta 80 sem expor o Node.js diretamente.

## Cenário 2 — Blog Corporativo 
A TechVision é uma consultoria de tecnologia em São Paulo. O time de marketing criou um blog estático (HTML/CSS puro) e quer que ele fique disponível publicamente. Porém, o gerente de TI tem uma exigência: deve haver dois virtual hosts diferentes no mesmo servidor Nginx:
blog.techvision.local → serve o site do blog
docs.techvision.local → serve uma página de documentação interna
Tudo isso dentro de um único container Nginx, gerenciado via Docker.
