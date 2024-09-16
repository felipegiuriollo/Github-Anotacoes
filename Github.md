- Git
    => Sistema de controle de versão

- Github
    => Plataforma online, que hospeda repositórios GIT. 
    - Existem outras plataformas como: bitbucket,gitlab, etc...


- GIT Comandos:
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
    