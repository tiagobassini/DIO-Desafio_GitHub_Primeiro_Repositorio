
# Configurando chave SSH para autenticação no git/github

### Gerar chave SSH
ssh-keygen -t ed25519 -C tiagobassini@gmail.com

- vai solicitar uma senha para a chave


### Pasta em que as chaves vao ser salvas
/c/Users/Meu Usuario/.ssh/


### Consultar valor da chave publica para add no github
$ cat id_ed25519.pub


### Exemplo de chave:
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIBH16w73uQ+Z3ktS5IHmUJpiVbonAeMjN9IimdHl6taj meu.email@gmail.com


### Inicializar Agent SSH para utilizar as chaves
$ eval $(ssh-agent -s)


### Passar chave privada para o SSH_Agent
ssh-add id_ed25519

- Informe a senha definida na criação da chaves

