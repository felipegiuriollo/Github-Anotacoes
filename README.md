- [x] Git
    - Sistema de controle de versão distribuído. É usado para rastrear alterações no código-fonte durante o desenvolvimento de software.

- [x] Principais Características Git  
    - Distribuído: Cada desenvolvedor possui uma cópia completa do repositório, incluindo seu histórico. Isso permite que o trabalho continue mesmo quando não há conexão com a rede.
    - Rastreamento de Alterações: Git registra cada alteração feita nos arquivos, permitindo voltar a versões anteriores e entender o histórico de mudanças.
    - Branching e Merging: Git facilita a criação de branches (ramificações) para trabalhar em novas funcionalidades ou corrigir bugs sem afetar a versão principal (branch principal, geralmente chamada de main ou master). Essas branches podem ser fundidas (merged) de volta ao branch principal.
    - Desempenho: Git é projetado para ser rápido e eficiente, lidando bem com grandes projetos e muitos arquivos.

- [x] Conceitos Git
    - Repositório (Repo): Local onde o projeto e seu histórico de versões são armazenados.
    - Commit: Registro de uma alteração no repositório. Inclui uma mensagem que descreve a mudança.
    - Branch: Linha de desenvolvimento independente. O branch principal geralmente é main ou master.
    - Merge: Processo de combinar alterações de diferentes branches.
    - Clone: Cópia local de um repositório remoto.

_____________________________________________________________________________________________________________________________________________

- [x] Github
    - Plataforma de hospedagem de código que usa Git como seu sistema de controle de versão.
        - Existem outras plataformas como: bitbucket,gitlab, etc...

- [x] Principais Características GitHub
    - Hospedagem de Repositórios: GitHub oferece um serviço na nuvem para armazenar repositórios Git, facilitando o acesso e a colaboração entre desenvolvedores.
    - Interface Web: Fornece uma interface gráfica que permite a navegação em repositórios, visualização de commits, criação de branches, e revisão de código.
    - Pull Requests: Mecanismo para revisar e discutir alterações antes de integrá-las ao branch principal. Permite feedback e colaboração antes da fusão de código.
    - Issues: Sistema de rastreamento de problemas e tarefas, permitindo que equipes gerenciem bugs e novas funcionalidades.
    - Actions: Ferramenta de CI/CD (Integração Contínua/Entrega Contínua) que permite automatizar fluxos de trabalho de build, teste e deploy.

- [x] Conceitos GitHub
    - Fork: Cópia de um repositório para a conta do usuário, permitindo modificar o código sem afetar o repositório original.
    - Pull Request (PR): Solicitação para integrar alterações de um branch ou fork ao branch principal, frequentemente acompanhada de revisão e discussão.
    - Gists: Repositórios simples para compartilhar trechos de código ou notas, úteis para pequenos projetos ou exemplos.

_____________________________________________________________________________________________________________________________________________

- [x] Como funcionam juntos:
    - Git é o sistema que realiza o controle de versão, enquanto GitHub é uma plataforma que facilita a colaboração e o gerenciamento de repositórios Git online.
    - Os desenvolvedores usam Git para fazer alterações e rastrear o histórico localmente. Quando querem compartilhar essas alterações com outros, ou colaborar em um projeto, eles fazem push de suas alterações para um repositório GitHub.
    - GitHub oferece ferramentas adicionais para colaboração, como pull requests e issues, que ajudam na gestão e revisão de código entre diferentes membros de uma equipe.

- [x] Resumo:
    - Em resumo, Git é a tecnologia que possibilita o controle de versão do código, enquanto GitHub é uma plataforma que hospeda esses repositórios e fornece ferramentas para colaboração e gerenciamento de projetos.

_____________________________________________________________________________________________________________________________________________


- [x] GIT Comandos:
    - git init: Inicializa um novo repositório Git vazio no diretório atual. Este comando cria uma nova pasta .git onde o Git armazenará todos os arquivos de configuração e histórico do repositório.
        - Uso: git init


    - git add .: Adiciona todos os arquivos e alterações no diretório atual ao "staging area" (área de preparação). Esses arquivos estão prontos para serem incluídos no próximo commit.
        - Uso: git add . -> Podendo também selecionar arquivos individualmente, como por exemplo git add "Commit_16_09_2024"


    - git commit -m "mensagem": Cria um commit, que é um ponto de verificação no histórico do repositório. A mensagem entre aspas deve descrever a mudança realizada no commit.
        - Uso: git commit -m "Descrição das mudanças"


    - git status: Exibe o status dos arquivos no repositório, incluindo arquivos modificados, não rastreados e prontos para o commit. Ajuda a entender quais mudanças estão por fazer o commit.
        - Uso : git status


    - git log: Mostra o histórico de commits do repositório, incluindo informações como o ID do commit, autor, data e a mensagem do commit. Pode ser usado para revisar o histórico de mudanças.
        - Uso: git log


    - git diff: Exibe as diferenças entre as versões dos arquivos no diretório de trabalho e a última versão commitada. Útil para ver quais mudanças foram feitas antes de um commit.
        - Uso: git diff


    - git restore <nome_arquivo>: Restaura um arquivo do diretório de trabalho para o estado do último commit. Esse comando desfaz mudanças não commitadas no arquivo especificado.
        - Uso: git restore <nome_arquivo>

    
    - git checkout -b <nome_da_branch>: Cria uma nova branch com o nome especificado e muda imediatamente para essa branch. Ideal para iniciar um novo ramo de desenvolvimento.
        - Uso: git checkout -b <nome_da_branch>


    - git branch: Lista todas as branches locais no repositório e indica a branch atualmente ativa (com um asterisco). Também pode ser usado para criar novas branches com a opção -b.
        - Uso: git bbranch


    - git checkout <nome_branch>: Muda para a branch especificada. Esse comando permite alternar entre diferentes ramos de desenvolvimento.
        - Uso: git checkout <nome_branch>


    - git merge <nome_branch>: Mescla as alterações da branch especificada na branch atualmente ativa. Normalmente usado para integrar alterações de uma branch de desenvolvimento (como uma feature branch) na branch principal (main ou master).
        - Uso: git merge <nome_branch>


    - git remote add origin <URL_repositorio>: Adiciona um repositório remoto com o nome origin e a URL fornecida. Usado para associar o repositório local a um repositório remoto, geralmente hospedado em serviços como GitHub, GitLab, ou Bitbucket.
        - Uso: git remote add origin <URL_repositorio>


    - git push origin <nome_branch>: Envia as mudanças da branch local para a branch correspondente no repositório remoto. Esse comando é usado para compartilhar suas alterações com outros colaboradores.
        - Uso: git push origin <nome_branch>


    - git pull origin master: Baixa e integra as alterações da branch master no repositório remoto para a branch local atual. Isso sincroniza seu repositório local com o repositório remoto.
        - Uso: git pull origin master


    - git fetch: Baixa todas as alterações do repositório remoto, mas não as integra automaticamente à branch local. Usado para atualizar o repositório local com novos commits e branches do remoto sem alterar o estado atual do seu diretório de trabalho.
        - Uso: git fetch

OBS: Esses comandos são fundamentais para trabalhar com Git e GitHub, oferecendo uma ampla gama de funcionalidades para gerenciar o histórico de código e colaborar em projetos.    

- [x] Resumo Comando:
    - git init -> Inicia novo projeto
    - git add . -> Pega todos os arquivos e adiciona em estado para commit
    - git commit -m "nome commit" -> Commita os arquivos no histórico
    - git status -> Mostra o status das alterações atuais
    - git log -> Vê todos os commits e informações sobre o commit
    - git diff -> Mostra todas a diferença do arquivo atual para o ultimo commit realizado, só mostra as diferenças antes do commit
    - git restore "nome arquivo" => Volta para a última versão
    - git checkout -b "nome da branch" -> Cria uma nova branch e vai direto para ela
    - git branch -> Mostra minha branch atual
    - git checkout "nome branch" -> Muda para outra branch
    - git merge "nome arquivo" -> Mesclar alterações de uma branch para MASTER(Ou de uma branch para outra)
    - git remote add origin "URL repositório" -> Adiciona um repositório remoto
    - git push origin "nome da branch" -> faz o envio da minha branch ao repositorio remoto
    - git pull origin master -> Traz todo o reposótio para minha máquina
    - git fetch -> Sincroniza todas as alterações remotas para o meu repositório local

Passo a passo para subir ao GITHUB (Não é regra!)
- git init -> Iniciando o git no projeto
    - git add . -> O ponto significa que ele vai deixar em estado de commit todos os arquivos modificados, mas pode usar o próprio nome do arquivo que você alterou. Ex: Meu arquivo se chama Commit_16_09_2024, pode usar da seguinte forma: git add Commit_16_09_2024
    - git commit -m '2024_09_16' -> Commita os arquivos no histórico
    - git remote add origin "URL do repositório criado no github" -> Adiciona um repositório remoto
    - git push origin "nome da branch" -> Enviando a minha branch ao repositório remoto

- Se por acaso você estiver dando o git push origin, e retornar o erro: remote origin already exists.
    - Significa que você já tem um repositório remoto criado, você pode continuar usando o mesmo ou optar por remover
        - Remover repositório remoto criado: 
         - git remote -v -> Mostra seus repositórios remotos criados
         - git remove remote 'nome repositório' -> Remover o repositório remoto criado