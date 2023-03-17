<h1 align="center">🔷 Poderoso 🔷</h1>


<div id="metadados" align="center">
    <img alt="Packagist Version" src="https://img.shields.io/packagist/v/dev-macb/poderoso?color=blue&logoColor=gray">
    <img alt="Packagist Downloads" src="https://img.shields.io/packagist/dm/dev-macb/poderoso?color=blue&logoColor=gray">
    <img alt="Packagist License" src="https://img.shields.io/packagist/l/dev-macb/poderoso?color=blue">
</div>


---

<h2 id="objetivo">🎯 Objetivo</h2>
<p>
O <strong>Poderoso</strong> é um pacote PHP que oferece uma abstração de banco de dados completa e fácil de usar. Com funções simples para configurar e conectar, é possível criar, ler, atualizar e excluir registros do banco de dados em poucos minutos.

Com o <strong>Poderoso</strong>, você não precisa mais se preocupar com a complexidade do acesso ao banco de dados. Ele oferece uma interface simples e intuitiva que permite que você crie, leia, atualize e exclua registros do banco de dados de forma rápida e fácil.

O <strong>Poderoso</strong> é compatível com as principais plataformas de banco de dados e é gratuito para uso em projetos comerciais e não comerciais. A documentação é clara e detalhada, tornando-o a escolha ideal para desenvolvedores que procuram uma solução confiável e fácil de usar para trabalhar com bancos de dados em projetos PHP.
</p>
<p align="center">🔷</p>


<h2 id="instalação">🔧 Instalação</h2>
<p>
    Para instalar o pacote <strong>Poderoso</strong>, certifique-se de que tenha o <a target="_blank" href="https://www.php.net/">PHP</a> e o gerenciador de pacotes <a target="_blank" href="https://getcomposer.org/">Composer</a> instalados em seu ambiente.
    Instale executando o seguinde comando:
</p>

```bash
$ composer require dev-macb/poderoso
```
<p>
    Para clonar o projeto para sua máquina via <a target="_blank" href="https://git-scm.com/">git</a>, execute os comandos a seguir:
</p>

```bash
$ mkdir poderoso && cd poderoso
$ git clone https://github.com/dev-macb/poderoso
$ composer install
```
<p align="center">🔷</p>


<h2 id="funcionalidades">⚙️ Funcionalidades</h2>
<p>
Para usar o Poderoso basta criar um arquivo <code>.env</code> na raiz de seu projeto. Como, por exemplo:

```env
BD_DRIV=mysql | pgsql
BD_HOST=localhost
BD_PORT=12345
BD_NAME=nome_do_banco
BD_USER=usuario_do_banco
BD_PASS=senha_do_usuario
```

Configure os dados de conexao com o banco de dados no arquivo <code>config.php</code>
```php
<?php
    use DevMacB\Poderoso;

    // Carregar .env na raiz do projeto
    Poderoso\BancoDados::configurar(
        getenv('BD_DRIV'),
        getenv('BD_HOST'),
        getenv('BD_PORT'),
        getenv('BD_NAME'),
        getenv('BD_USER'),
        getenv('BD_PASS'),
    );
?>
```
<blockquote>
    Lembre-se de adicionar no <code>.gitignore</code> as arquivos de variáveis de ambiente para não colocar dados sensíveis do seu projeto para repositórios na nuvem
</blockquote>

<p align="center">🔷</p>



<h2 id="contribuições">✒️ Contribuições</h2>
<p>
    Toda contribuição será bem-vinda!🎉 Caso tenha encontrado algum bug, propor uma nova funcionalidade ou conversar sobre o projeto <a href="https://github.com/dev-macb/poderoso/issues">Abra uma Issue</a> e descreva seu caso. Se houver uma issue aberta e você deseja resolve-la, adicionar uma nova funcionalidade ou melhorar a documentação, desenvolva suas adições e me envie um <em>Pull Request</em>. Gostou do projeto e ainda não consegue contribuir com ele? Considere deixar uma ⭐ para o <strong>Ambivar</strong>. Desde já agradeço pelo interesse em colaborar de alguma forma com o nosso projeto.</a>
</p>
<p align="center">🔷</p>



<h2 id="licença">📄 Licença</h2>
<p>
    O Poderoso utiliza a <strong>licença MIT</strong> em todo seu código, confira suas condições em <a href="https://github.com/dev-macb/poderoso/blob/dev/LICENSE.md">LICENSE</a>.
</p>
<p align="center">🔷</p>