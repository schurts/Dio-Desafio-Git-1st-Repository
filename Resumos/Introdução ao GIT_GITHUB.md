Aula 1 - Entendendo o que é Git e sua importância

- Git é um sistema de versionamento de códigos distribuídos
  - Benefícios
    - Controle de versão
      - Foco principal
    - Armazenamento em nuvem
      - Dos códigos
    - Trabalho em equipe
      - Potencializa
    - Melhorar seu código
      - Com a disponibilização do seu código, qualquer outra pessoa pode utiliza-lo assim melhorado
    - Reconhecimento

Aula 2 - Navegação via command line interface e instalação

Etapa 1 - Comandos básicos para um bom desempenho no terminal

- Interação com Windows
  - CD
    - Possibilita que navegue pelas pastas
  - DIR
    - Lista as pastas aonde esta situada
  - MKDIR
    - Cria uma pasta
  - DEL / RMDIR /s /q
    - Deleta arquivos solicitados e tudo dentro das pastas
  - CLS
    - Limpa o cmd
- Interação Unix
  - CD
    - Possibilita que navegue pelas pastas
  - LS
    - Lista as pastas aonde esta situada
  - MKDIR
    - Cria uma pasta
  - RM -RF
    - Deleta arquivos solicitados e tudo dentro das pastas
  - CLEAR
    - Limpa o cmd

Etapa 2 - Realizando a instalação do GIT

- Realizado kk

Aula 3 - Entendendo como o GIT funciona por baixo dos panos.

Etapa 1 - Tópicos fundamentais para entender o funcionamento do Git

- Conceitos
  - SHA1
    - SHA(Secure Has Algorithm) é um conjunto de funções hash criptográficas projetada pela NSA
    - A encriptação gera um conjunto de caracteres identificador de 40 dígitos(stdin)
    - É uma forma curta de representar um arquivo
  - Objetos fundamentais
    - Blobs
    - Tress
    - Commits
  - Sistema distribuído
  - Segurança

Etapa 2 - Objetos internos do Git

- Blobs
  - Contém meta dados GIT, assim sabendo o tamanho do arquivo, tipo do objeto etc.
- Trees
  - As Trees armazena os Blobs, também contém meta dados, ela também guarda o nome do arquivo, diferente dos Blobs,
- Commits
  - Mais importante de todos, objeto que junta tudo, da sentido a tudo que está sendo feito, também possui SHA1,

Etapa 3 - Chave SSH e Token

- Chave SSH
  - É uma conexão segura e encriptada em duas máquinas, criando uma chave pública e privada.
- Comandos
  - Criar chave
    - ssh-keygen -t ed25519 -C “email”
      - Se atentar a letras minúsculas e maiúsculas
  - SSH ENGINE
    - Identidade responsável por pegar as chaves e lidar com elas
      - eval $(ssh-agent -s)
        - O numero gerado é condizente como número de estresse e impacto no PC (ele está rodando por trás)(lá ele)
    - Adicionar a chave
      - ssh-add id_ed25519 e senha
- Git clone
  - Usado para clonar uma ssh

Aula 4 - Primeiros comandos com Git

- Iniciando o Git e criando um commit
  - Comandos
    - git init
      - Iniciar o repositório
    - gt add
      - Mover arquivos e dar inicio ao versionamento
    - git commit
      - Criar um commit
  - Criando um repositório
    - -a : mostra pastas ocultas
    - git config --global [user.email](http://user.email) “email” : Cadastrando inicialmente no Git com o email
    - git config --global [user.name](http://user.name) “name” : Cadastrando inicialmente no Git com o nome
    - Arquivo markdown
      - Uma forma mais humana de se escrever um arquivo HTML
    - HTML : é o esqueleto, estrutura básica de toda página na WEB.
    - git add *
    - git commit -m (para criar o commit inicial)

Aula 5 - Ciclo de vida dos arquivos Git

- Passo a passo do ciclo de vida
  - Git Init
    - Cria o depositório
  - Tracked(temo ciencia)
    - Pode se dividir em 3 colunos diferentes
      - Unmodified
      - Modified
      - Staged
  - Untracked(não temos ciencia)
  - Git add
    - Adiciona o arquivo, movendo untracked para Staged, aonde está aguardando para ser utilizado
  - Modified
    - Aonde detecta que está sendo editado
    - Aonde é modificado salvo e vai pra Staged novamente
  - Unmodified
    - Quando não é modificado, se excluido ele vai para untracked.
  - Staged
    - Quando está se preparando para um commit, quando “envelopamos tudo em um commit” ele deixa de ser staged pra commit e posteriormente vira modified.

Aula 7 - Como os conflitos acontecem no GiftHub e como resolve-los

- 