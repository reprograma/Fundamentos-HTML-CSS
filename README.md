# HTML e CSS Básicos

[Documentação HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML)


# Comandos git
```
git init
```
Cria um arquivo .git dentro da sua pasta local, estabelecendo a conexão com o git. Dentro deste arquivo ficará toda a informação de versionamento.


```
git config --global user.name "seu-username"
git config --global user.email "seu-email@provedor.com"
```
Para logar com seu usuário na CLI. 

```
git config --global --unset-all user.name "seu-username"
git config --global --unset-all user.email "seu-email@provedor.com"
```
Para deslogar seu usuário na CLI. Lembre-se de checar se o Windows está considerando esse usuário em:

````Painel de controle / Contas de Usuário / Gerenciar credenciais do Windows /````

```
git remote add origin <url-do-repositório>
```
Para atrelar a pasta local do repositório no Github

```
git remote -v
```
Para verificar a qual repositório a pasta local está atrelada

```
git status
```
Para listar todas as modificações feitas desde o último commit

```
git pull origin master
```
Para atualizar sua pasta local com a versão atual do repositório remoto

```
git add <arquivos-a-adicionar>
git add .
```
Para adicionar arquivo por arquivo ou todos os arquivos modificados

```
git commit -m 'Sua mensagem aqui'
```
Para enviar alterações que você acabou de adicionar para a HEAD

```
git push origin master
```

Para enviar commits para o repositório remoto (na branch master)