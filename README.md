# Material de estudo

Cada pasta conta com os exercício para cada dia da semana de aula. Aqui você vai encontrar o layout a ser desenvolvido e a resolução dos exercícios. Ao longo da semana, vou adicionar um README para cada dia, com links de estudo e material que discutimos em aula.

# Dúvidas

Para tirar dúvidas, leve para a sala de aula, mande mensagem para a professora ou abra um issue aqui no repositório.

# HTML e CSS Básicos

[Documentação HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML)

[Documentação CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS)


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

# Método BEM

Forma de nomear as classes do CSS seguindo um padrão fixo baseado em Blocos, Elementos e Modificadores. Oferece 3 principais benefícios:


* Traduz claramente a **estrutura** da página
* Torna possível ter estilos **reutilizáveis**, sem precisar ficar repetindo os mesmos estilos em vários elementos
* Torna seu código **modular**, ou seja, evita que estilos sejam passados "sem querer" por meio da cascata.


Para seguir o padrão BEM, basta seguir o seguinte formato para nomear suas classes:

```
bloco__elemento--modificador
```

**Bloco** é tudo aquilo que representa um componente independente da página. Possui um sentido se usado sozinho e pode ser reutilizado.
*Ex: menu, botão, formulário*


**Elemento** é tudo aquilo que ajuda a construir o componente independente. Ou seja, se colocado sem uma "mãe" e sem "irmãos" não funciona bem.
*Ex: item da lista, campo do formulário*


**Modificador** é tudo aqui que varia entre elementos ou componentes que podem ser iguais. Por exemplo, quando temos vários botões em uma página e um deles tem a cor diferente. Ele continua sendo um botão, mas precisa ser diferenciado dos outros. É sempre uma característica ou estado.
*Ex: botão vermelho, menu horizontal ou vertical*


> Importante: podemos usar modificadores tanto com elementos quanto com blocos diretamente.


Exemplos válidos:

```
conteudo__item
conteudo__item-visitado
```

```
menu__item
menu--horizontal
```
