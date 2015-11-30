# Instala mongo-hacker Windows

Comecei o curso ontem e tive um grande problema com o mongo-hacker, passei tarde toda procurando uma solução e finalmente achei. E estou aqui para compartilha-la com vocês para começar já deveremos ter:

  - git e gitbash
  - nodejs
  - mongo

Então vamos começar baixando o comando make que o "Ruindows" não nos oferece nativamente, eu recomendo o [GNUWIN ](https://github.com/user/repo/blob/branch/other_file.md) basta baixar 'Complete package, except sources'. Depois de baixa-lo e instalalo vamos adiciona o arquivo no Path.

Primeiro vamos procurar a pasta raiz onde se localiza o make geramente fica em 
"C > Program Files (x86) > GnuWin32 >bin" resumindo "C:\Program Files (x86)\GnuWin32\bin"

![alt tag](http://i.imgur.com/KjWOlNy.png)

caso voce ache um ícone chifrudo com nome maker deu tudo certo basta copiar url.Então vamos ao host caso você use Windows 8, 8.1 e 10 siga este passo caso use outra versão pesquise no PaiDosBurros(Google) "Como mudar o PATH nos Windows". quem usa o 8, 8.1 e 10 siga em frente

click com o botão direito do seu mouse na bandeira do Windows.
![alt tag](http://i.imgur.com/ihc8NHy.png)

click em sistema

![alt tag](http://i.imgur.com/pvOPXK8.png)

clique em Configurações Avançadas

![alt tag](http://i.imgur.com/fsAymza.png)

variáveis de ambiente...

![alt tag](http://i.imgur.com/kXxgsf8.png)

selecione path e clique em editar

![alt tag](http://i.imgur.com/hW31Hl7.png)

vá ate final da linha coloque um ; no final caso não aja e cole o diretorio que nos acho lá em cima

![alt tag](http://i.imgur.com/lrgWeed.png)

pronto instalamos o make no Windows agora vamo testa abra o GIT BASH pelo amor de tudo que e mais sagrado, Nao use o CMD(aquela porcaria). Com o git bash aberto digite

```sh
$ make
```

![alt tag](http://i.imgur.com/b4Tnhc2.png)

caso receba essa mensagem tudo deu certo, caso não aparece essa messagem reinicia windows e digite denovo. 

agora vamos instala o mongo-hacker. Primeiro clone o repositorio na pasta dos repositórios do npp para organiza 

```sh
$ cd 'C:\Users\wesll\AppData\Roaming\npm\node_modules'
```

obs: caso a pasta node_modules não exista, você deve cria-la

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

clone o repositório

```sh
$ git clone https://github.com/TylerBrock/mongo-hacker.git
```

agora vamos configura lo para não ficar exibindo umas mensagens de erro chata

```sh
$ cd mongo-hacker
```

```sh
$ notepad config.js
```

agora vamos mudar duas variaveis á windows_warning e force_color 
a windows_warning ficara false e force_color true 

![alt tag](http://i.imgur.com/GowCCAl.png)

agora so instalar o mongo hacker com o

```sh
$ make install
```

pronto mongo-hacker instalado com sucesso

![alt tag](http://i.imgur.com/xEx3QKW.png)

aeeeeeeeeeee agora nosso console fico 'bunitinho'

galera desculpem-me os erros de portugues, fiz na intenção de ajudar mas vo arumando isso e commitando..
