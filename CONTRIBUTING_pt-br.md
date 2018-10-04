# Guia de Contribuição

COMO CONTRIBUIR COM CÓDIGO ABERTO aceita PR's (pull requests) de **novatos**
apenas, isso é para que os **novatos** ganhem familiaridade com o processo
de contribuição.

As issues podem ser submetidas por qualquer pessoa, desenvolvedores experientes
ou iniciantes.

### Iniciando

1.  Se você tem pouca experiência com Git e Github, aconselha-se que você veja [esse link](http://readwrite.com/2013/09/30/understanding-github-a-journey-for-beginners-part-1/)
    antes de seguir para o próximo passo.

2.  Faça um fork do projeto no Github, [Guia de ajuda para fazer fork de um repositório](https://help.github.com/articles/fork-a-repo/).
[![Screen Shot 2016-10-06 at 11.46.47 PM.png](https://s13.postimg.org/5yvhu7vpz/Screen_Shot_2016_10_06_at_11_46_47_PM.png)](https://postimg.org/image/6oea6kw9f/)
3.  Clone o projeto.
4.  Crie uma branch específica para a issue na qual você vai trabalhar.

    ```shell
    git checkout -b update-readme-file
    ```

    Para clareza, para você mesmo e outros, sobre qual issue você está
    trabalhando, nomeie sua branch como `update-xxx` ou `fix-xxx` onde o
    `xxx` é uma curta descrição do que você está fazendo. Por exemplo,
    `update-readme` ou `fix-typo-on-contribution-md`.

5.  Abra seu projeto no seu editor desejado, selecione o arquivo que quer
    trabalhar e faça suas mudanças.
    
    Se você está alterando o arquivo README.md, será necessário entender sobre
    Markdown. Visite [esse link para ler sobre Github
    Markdown](https://guides.github.com/features/mastering-markdown/) e [esse
    para praticar](http://www.markdowntutorial.com/)

    *   Se você está adicionando um projeto ou organização nova ao README,
        certifique-se de manter a lista em ordem alfabética.
    *   Se você está adicionando uma nova organização, garanta que haja um
        rótulo (label) para o nome da organização. Isso facilitará distinguir
        projetos de projetos de organizações.

6.  Quando terminar suas mudanças em sua branch nova, adicione os arquivos
    necessários no git, [Como faze add, commit, push e
    go](http://readwrite.com/2013/10/02/github-for-beginners-part-2/)

    ```shell
    git add caminho/para/arquivo.ext
    ```

    Você também pode adicionar todos os arquivos usando:

    ```shell
    git add .
    ```

    Cuidado, pois ao usar `git add .` você adicionará automaticamente todos os
    arquivos. Com `git status` você consegue ver suas mudanças, mas faça antes
    de `git add`.

6.  Faça o commit de suas mudanças com uma mensagem descritiva no seu commit.

    ```shell
    git commit -m "Breve descrição do commit"
    ```

7.  Faça o push de seus commits para seu fork no github:

    ```shell
    git push -u origin nome-da-branch
    ```

8.  Submeta um pull request.

    Dentro do Github, visite o repositório principal e você deve ver um banner
    sugerindo a criação de um pull request. Ao criar um pull request, pode ser
    adicionado um `Closes #XXX` ao corpo da mensagem, onde `#XXX` é a issue que
    você está consertando. Então, como exemplo, seria `Closes #42` para fechar
    a issue `#42`.


### Submetendo um Pull Request

O que é um pull request?
[Visite esse link (em inglês)](https://yangsu.github.io/pull-request-tutorial/)

Se você deseja cuidar de uma issue, aconselha-se que você verifique o conteúdo
dos comentários na issue, caso alguém já esteja trabalhando nela. Se ninguém
estiver trabalhando na issue no momento, gentilmente deixe um comentário
informando sua intenção de trabalhar nela, desse modo evitará que outras 
pessoas façam esforço duplicado do seu trabalho.

Numa situação onde alguém se candidatou para cuidar de uma issue, mas não houve
nenhuma atualização por um perído específico, tipo 2-3 semanas, é aceitável que
você ainda pegue essa issue, mas lembre-se de deixar um comentário antes.

*Nota*: Todo projeto open-source tem um arquivo **CONTRIBUTING.md**, por favor
leia esse aquivo antes de abrir um pull request, ou então há o risco de seu
pull request ser rejeitado. Entretanto, caso ainda não exista um arquivo
CONTRIBUTING.md, você ainda pode criar um pull request mas o faça de modo
descritivo.

### Links úteis (em inglês)

- [Pro GIT Book](https://git-scm.com/book/en/v2)

- [Try Git](https://try.github.io/)
