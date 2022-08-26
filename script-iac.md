# script no terminal ubuntu NANO

```
#!/bin/bash

echo "atualizando o servidor..."
apt-get update
apt-get upgrade -y
apt-get install apache2 -y
apt-get install unzip -y
```
```
echo "baixando e copiando arquivos da aplicação..." 
cd /tmp
wget https://github.com/marehead/Infraestrutura-como-Codigo-Script-de-Provisionamento-de-um-Servidor-Web-Apache-.git
unzip main.zip
cd linux-site-dio
cp -R * /var/www/html/
```

ctrl+o  para salvar 
ctrl+x sair do nano
chmod +x [nome do arquivo] para dar permissão
