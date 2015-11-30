# Instala mongo-hacker Windows

Comecei o curso ontem e tive um grande problema com o mongo-hacker, passei tarde toda procurando uma solução e finalmente achei. E estou aqui para compartilha-la com vocês para com essa já deveremos ter:

  - git e gitbash
  - nodejs
  - mongo

Então vamos começar baixando o comando make que o "Ruindows" não nos oferece nativamente, eu recomendo o [GNUWIN ](https://github.com/user/repo/blob/branch/other_file.md) basta baixar 'Complete package, except sources'. Depois de baixa-lo e instalalo vamos adiciona o arquivo no Path.

Primeiro vamos procurar a pasta raiz onde se localiza o maker geramente fica em 
"C > Program Files (x86) > GnuWin32 >bin" resumindo "C:\Program Files (x86)\GnuWin32\bin"

![alt tag](http://i.imgur.com/KjWOlNy.png)

caso voce ache um incone chifrudo com nome maker deu tudo certo basta copiar url.Então vamos ao host caso você use Windows 8, 8.1 e 10 siga este passo caso use outra versão pesquise no PaiDosBurros(Google) "Como mudar o PATH nos Windows". quem usa o 8, 8.1 e 10 siga em frente 

clic com o botão direito do seu mause na mandeira do Windows.
![alt tag](http://i.imgur.com/ihc8NHy.png)

clikc em sistema 

![alt tag](http://i.imgur.com/pvOPXK8.png)

clique em Coniguração Avançadas

![alt tag](http://i.imgur.com/fsAymza.png)

variaveis de ambiente...

![alt tag](http://i.imgur.com/kXxgsf8.png)

selecione path e clique em editar

![alt tag](http://i.imgur.com/hW31Hl7.png)

vá ate final da linha coleque um ; no final caso não aja e cole o diretorio que nos acho lá em cima

![alt tag](http://i.imgur.com/lrgWeed.png)

pronto intalamos o make no Windows agora vamo testa abra o BIT BASH pelo amor de tudo que e mais sagrado, Nao use o CMD(aquela porcaria). Com o git bash aberto digite 

```sh
$ make
```

![alt tag](http://i.imgur.com/b4Tnhc2.png)

caso esiba essa messagem tudo deu certo, caso não aparesa essa messagem reinicia windows e digite denovo. 

agora vamos instala o mongo-hacker. Primeiro clone o repositorio na pasta dos repositorios do npp para organiza 

```sh
$ cd 'C:\Users\wesll\AppData\Roaming\npm\node_modules'
```

obs: caso a pasta node_modules não esita criea 

```sh
$ cd 'C:\Users\wesll\AppData\Roaming\npm\'
```

```sh
$ mkdir node_modules
```

```sh
$ cd node_modules
```

dentro da pasta node_modules no terminal

clone o repositorio

```sh
$ git clone https://github.com/TylerBrock/mongo-hacker.git
```

agora vamos configuralo para não fica esibibo umas messagens de erro chata

```sh
$ cd mongo-hacker
```

```sh
$ notepad config.js
```

agora vamos mudar duas variaveis á windows_warning e force_color 
a windows_warning ficara false e force_color true 

![alt tag](http://i.imgur.com/GowCCAl.png)

agora so intala com o 

```sh
$ make install
```

pronto mongo-hacker intalado com sucesso 

![alt tag](http://i.imgur.com/xEx3QKW.png)

aeeeeeeeeeee agora nosso console fico 'bunitinho'

galera descupe-me os erros de portugues, fiz na intenção de ajudar mas vo arumando isso e commitando..
