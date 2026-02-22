## Converter chave de .ppk para .pem

sudo pacman -S putty
xxxx
xxxx

## Logar no servidor com chave e usuário repassados

## Atualizar servidor e instalar curl, Docker e Jenkins

sudo apt update && sudo apt upgrade -y
https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository

### Jenkins:

https://www.jenkins.io/doc/book/installing/linux/#debianubuntu

sudo cat /var/lib/jenkins/secrets/initialAdminPassword
97\*\*\*\*db

978f6b10366a44ed968ed53dd03e3edb

## Criar pastas do Jenkins (server e agents)

mkdir -p ~/jenkins/{server,agent1,agent2}
cd ~/jenkins

## Docker-compose

https://docs.docker.com/compose/gettingstarted
https://www.jenkins.io/doc/book/pipeline/docker/

## Criar usuário e senha no jenkins (evitar usar admin)

Você pulou a configuração do usuário admin.

Para entrar, use o nome de usuário "admin" e a senha de administrador que você usou para acessar o assistente de configuração.

Bloquear portas (exceto 8080 e ssh)
sudo ufw allow ssh xxxxx 8080/tcp
sudo ufw enable
sudo ufw status
