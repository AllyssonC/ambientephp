# Descrição

Este ambiente é destinado a ser utilizado nas aulas de PHP ministradas pelo prof Jeferson Rodrigo Almeida.

Recomenda-se que seja realizado um *fork* do projeto para o seu próprio github (se não tem uma conta, [crie agora mesmo](https://github.com/join?source=header-home)), para então clonar a partir do seu projeto. É possível apenas clonar o projeto, mas vocẽ não será capaz de realizar ações de *push* para ele, por isso esse formato não é recomendável.

Utilizando corretamente o *git*, além de ter controle sobre tudo que é realizado em seus projetos, você simplifica muito o trabalho em equipe, e tem um backup extremamente confiável dos seus projetos.

Esse projeto será atualizado constantemente, sempre que for necessário qualquer alteração no ambiente, por isso é recomendável realizar constantemente uma [sincronização](https://help.github.com/articles/syncing-a-fork/) do seu *fork*.

Qualquer dúvida no processo, o professor deve ser consultado em sala de aula.


# Subindo o ambiente

Além do projeto clonado, você deve ter os seguintes pré-requisitos instalados para que o ambiente funcione:

* [Vagrant](https://www.vagrantup.com/docs/installation/)
* [Oracle VM Virtualbox](https://www.virtualbox.org/wiki/Downloads)
* [Ansible](http://docs.ansible.com/ansible/intro_installation.html)

O sistema operacional recomendado é o Linux, mas todas as dependências são portáveis para vários sistemas operacionais, incluindo Windows, MacOS e diversas distribuições de Unix e Linux.

O sistema de virtualização pode ser qualquer um suportado pelo Vagrant. Alguns (como por exemplo o VMWare), dependem de software adicional ser instalado. Recomenda-se o Oracle Virtualbox, e é para esse *provider* que o ambiente está configurado (no caso de uso de outro *provider*, será necessário ajuste na configuração do ambiente).

Uma vez instaladas todas as dependências, deve-se rodar na raiz do projeto (mesma pasta deste arquivo), o seguinte comando:

    $ vagrant up

O *Vagrant* vai criar o ambiente. Em caso de erros consulte o professor.

O download do *box* (instalador do Ubuntu Server 14.04) pode demorar muito tempo, dependendo da sua conexão com a internet. Se preferir solicite durante a aula que o professor passe via pen drive o arquivo compactado com o *box*, e peça as instruções para incluí-lo no seu ambiente antes de subir o vagrant.

Uma vez criado o ambiente, vocẽ pode:

## Acessar o ambiente via shell:

    $ vagrant ssh


## Acessar o projeto pelo navegador:

    http://localhost:9000


## Alterar o código PHP do ambiente:

O código do projeto está na pasta **src**. O *Vagrant* automaticamente mapeia todos os arquivos desta pasta para o document root do servidor virtual.


## Administrar o servidor Virtual:

    $ vagrant help
    $ vagrant version
    $ vagrant up
    $ vagrant ssh
    $ vagrant provision



