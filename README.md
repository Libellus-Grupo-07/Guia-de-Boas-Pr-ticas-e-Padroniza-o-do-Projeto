# Guia de Boas Práticas e Padronização do Projeto

Este guia tem como objetivo estabelecer diretrizes e padrões para o desenvolvimento de projetos neste repositório. Siga estas práticas recomendadas para garantir a consistência, legibilidade e qualidade do código.

1. Estrutura do Projeto.
   
Mantenha uma estrutura de diretórios organizada e consistente para facilitar a navegação e a manutenção do projeto.
Separe o código-fonte, os recursos e a documentação em diretórios distintos.
Utilize um sistema de controle de versão, como o Git, para rastrear as alterações no código.

2. Convenções de Nomenclatura

Utilize nomes descritivos para variáveis, funções, classes e arquivos.
Siga as convenções de nomenclatura recomendadas para a linguagem de programação usada no projeto.
Evite abreviações e nomes genéricos. Priorize a clareza e a legibilidade do código.

3. Comentários e Documentação

Documente o código de forma clara e concisa, explicando a finalidade, o comportamento e a utilização de cada função, classe e método.
Adicione comentários relevantes para esclarecer partes complexas ou pouco intuitivas do código.
Mantenha a documentação atualizada à medida que o projeto evolui.

4. Estilo de Código

Siga um estilo de código consistente em todo o projeto.
Utilize indentação adequada para melhorar a legibilidade.
Evite linhas muito longas, que podem dificultar a leitura. Se necessário, quebre as linhas de acordo com as convenções estabelecidas para a linguagem.

5. Testes Unitários

Escreva testes unitários para verificar o comportamento esperado das funções e métodos do projeto.
Automatize a execução dos testes para que possam ser facilmente executados durante o desenvolvimento e a integração contínua.

6. Controle de Dependências

Utilize uma ferramenta de gerenciamento de dependências adequada para a linguagem utilizada (por exemplo, npm para JavaScript, pip para Python).
Mantenha um arquivo de manifesto (como o package.json ou requirements.txt) para listar todas as dependências do projeto, incluindo as versões específicas.

7. Segurança

Esteja atento às práticas de segurança recomendadas ao lidar com dados sensíveis, como senhas e informações pessoais.
Evite vulnerabilidades conhecidas e mantenha todas as dependências atualizadas com as versões mais recentes.
Realize revisões regulares de segurança e corrija quaisquer problemas identificados.

8. Utilização de branch

Para utilizar o git hub seguindo alguns conceitos que adquiri com o pessoal da Sptech, escrevi a sequência de comandos (para quem usa o terminal do git) para utilizar o git hub, em dois casos:
1)para quem não tem a Branch criada:
Cria o repositório/branch -> git init
Altera o nome da Branch -> git branch -m <nome Branch atual> <novo nome da Branch>
Realiza a conexão da Branch com o repositório -> git remote add <nome da Branch> <link do repositório>
Confira se está na Branch certa -> git status
Gera o pacote de alterações/arquivos -> git add .
OBS: É possível utilzar mais de 1 'git add .', smepre será adicionado ao pacote
para fechar o pacote -> git commit -m '<comentário>'
OBS: O '-m' serve para registrar a mensagem de commit. Exe: Git commit -m 'Ajuste na classe De Teste'
para enviar o pacote ao git -> git push --set-upstream <nome da Branch> <nome da branch>
OBS: Esse comando é para definir a Branch para receber push, execute somente na primeira vez, nas próximas vezes, utilize o 'git push'//
//--set-upstream : É usada para configurar a branch remota como upstream da branch local.
2) Para quem já tem a Branch criada:
Clona a pasta do repositório -> git clone <link do repositório>
Entra na pasta clonada -> cd <nome da pasta>
Acessa a Branch -> git checkout <nome da Branch>
Confira se está na Branch certa -> git status
git add .
OBS: É possível utilzar mais de 1 'git add .', smepre será adicionado ao pacote
para fechar o pacote -> git commit -m '<Comentario>'
OBS: O '-m' serve para registrar a mensagem de commit. Exe: Git commit -m 'Ajuste na classe De Teste'
para enviar o pacote ao git -> git push

9. Commitar qualquer alteração

Não importa qual foi a alteração, é importante que dê commit no que foi feito (mesmo que uma implementação simples e pequena). Isso se deve ao fato de que todo dia todos deverão dar um git pull, então é necessário subir todas as alterações para que não haja conflitos.
