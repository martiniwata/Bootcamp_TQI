# 02 - Introdução ao Git e ao GitHubt :man_technologist:



### Anotei os seguintes pontos: 

* O Git é um software de versionamento de código Local, usado para que vários usuários consigam editar o mesmo arquivo, onde as diferenças das edições são identificadas em caso de conflito (edição na mesma linha) :heavy_check_mark:

* O GitHub é um repositório Remoto de versionamento de código. Ele receberá as edições feitas e enviadas pelo Git (solução local) e as deixarão disponíveis na nuvem :heavy_check_mark:

* Eles usam a codificação SHA1, o qual fornece uma assinatura da versão (uma assinatura de 40 caracteres). Qualquer edição feita no arquivo fará com que seja feito uma nova assinatura :heavy_check_mark:

* Para usar o Git, entrar no site próprio (git.com) e baixar a versão mais atual, onde após a instalação, usar o Git Bash :heavy_check_mark:

  

### Dados do Git:

- Após instalado, usar o Git Bash :heavy_check_mark:
- Dentro do Git Bash, usar os comandos da linha de comando, seja do Windows como do Linux :heavy_check_mark:
- Usar o comando:   git init  (vai criar um repositório na pasta que vc estiver) :heavy_check_mark:
- Usar o comando:  git add  (depois que vc criar arquivos, com esse comando vc os colocarão na fila do commit) :heavy_check_mark::question:
- Se usar o comando git add NomeArquivo.Extensão vc manda só esse arquivo. Se escrever git add *  ele vai mandar todo o arquivo do seu repositório (lembra do init?) :heavy_check_mark:
- Usar o comando git commit -a "breve descrição do que vc alterou neste comiit"  (vai salvar os arquivos com que vc colocou, versionando-os, claro, após vc ter dado o git add. Com isso ele já faz uma assinatura do arquivo) :heavy_check_mark:
- Usar o comando git status  (ele mostra em que pé está o seus arquivos, se já foram salvos, estão comitados, etc) :heavy_check_mark::heavy_check_mark:
- 

### Dados Git | GitHub

- Agora que está commitado os seus arquivos, você precisa salvá-los no seu repositório remoto, para que esteja visível para os demais usuários, possa ser editado, etc :heavy_check_mark:
- Antes de mais nada, entre em github.com e crie uma conta de usuário, para evoluir com os estudos (preencha todos os campos e faça todas as validações) :heavy_check_mark:
- Após a criação do usuário, não esqueça de instalar e ativar a chave SSH nos computadores que forem utilizados para alimentar o GitHub :heavy_check_mark:
- Para isso, entrar em sua foto/Settings (vai abrir uma página de configuração). No canto esquerdo, sleecionar "SSH and GPG Keys" (vai abrir uma nova tela). Depois disso, vá em "New SSH Key" (é nessa tela que jpga a chave criada) :heavy_check_mark:
- Quando estiver nessa tela, entrar em seu computador no programa git bash para criar as chaves executando o comando:   ssh-keygen -t ed25519 -c martin.iwata@hotmail.com    :thinking:**seu email ** :heavy_check_mark:
- Ao executar o comando, será perguntado sobre o caminho que será salvo (manter o padrão, dentro de C:\Users\Martin  :thinking:**seu Usuário Atual**) :heavy_check_mark:
- Depois de terminado a criação da chave, vá na pasta onde foi criada, onde precisará visualizar a chave (usar o comando cat NomeDaChavePublica) :heavy_check_mark:
- Copia a sua chave e cole dentro do gitHub (naquela tela que estamos), onde o título vc pode coloque de uma forma que vc reconheça o computador depois (ex: Computador Casa, etc) :heavy_check_mark:
- Dê o add na chave (deve pedir a sua senha do github) :heavy_check_mark:
- Depoís disso vá  no git bash novamente e execute o comando:   eval $(ssh-agent -s) :heavy_check_mark:
- Por fim, digite o comando pra amarrar a sua chave privada ao agente ativado:   ssh-add if-25519 :heavy_check_mark:
- Com o fim da criação da chave SHH, precisará configurar os dados para o envio do commit. Digite o comando:   git config --global user.email "seu email usado no github"
- Usar também este comando para adicionar o nome de usuário:   git config --global user.name "seu nome de usuário usado no github" :heavy_check_mark:
- Depois disso vc cria um repositório dentro do github (clica na sua foto/new repository), adicionando um nome que tenha a ver com o seu projeto :heavy_check_mark:
- Com o repositório criado no github, copie o endereço https disponível no seu repositório (vai aparecer quando vc terminar de criar)  "...or push an existing repository from the command line":heavy_check_mark:
- No seu git bash, precisa adicionar a origem (que é o github):      git remote add origin **endereço do repositório copiado acima!!** :heavy_check_mark:
-  Vc digitando    git remote -v   vai aparecer a lista de repositórios cadastrados!!
- Depois você usará o comando:    git push origin master  (esse comando vai empurrar os seus códigos locais para o repositório remoto. Vai precisar dos seus dados de acesso do github) :heavy_check_mark:
- Se tiver algum conflito com alguma versão (duas pessoas editaram a mesma linha de código, informará a situação, para você resolver as diferenças e deixar a versão mais atual) :heavy_check_mark::heavy_check_mark:



### :space_invader: Terminei a matéria finalizando o teste final em 4 minutos e 30 sergundos (de um total de 12 minutos), com 80% de acerto.



![Success-PNG-Background-Image](D:\#ESTUDOS\Bootcamp TQI Dev Fullstack\20-ImagensUsadas\Success-PNG-Background-Image.png "Comemoração")



