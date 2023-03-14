# Comandos Git

#### OBS:

- **Cntrl + L**: Atalho de limpeza de código na tela
- Markdown **(extensão .md)**: forma humana de usar HTML
- Nome de branch aceita traço! (**-**)

---

cd nome-do-repositório: Para entrar na pasta

---

**git init**: Criar repositório

**git config --global user.email "rebecab.silva98@gmail.com"**: Configurar para primeiro uso (atribuir autor)

**git config --global.name Rebeca**: Configurar nome

**git clone link.com**: Clonar um projeto do GitHub

**git checkout -b**: Cria uma branch nova e se move até ela

**git status**: Para verificar o status do código em relação ao GitHub

**git add***: Adiciona todas as modificações pra staged para poder comitar
- git add .
- git add -a

**git remote add origin link.com**: Criar repositório no GitHub e upar projeto do PC pra lá

**git push origin main**: Empurrar para o GitHub

**git pull origin main**: Puxar para o PC

**git commit -m "alterações fazem"**: Commitando

**git branch**: Ver as branches no repositório local

**git branch -m nome-novo**: Renomear a branch estando dentro dela

**git branch -m nome-antigo nome-novo**: Renomar a branch estando fora dela

**git branch -d nome-da-branch**: Deletar branch

---

> stach

**git stach save "fazendo alterações"**
- Stach é um Array [0]
**git stach list**: Mostra a lista dentro do Array

**git stach pop 1**: Estourar a caixinha e voltar a trabalhar

**git stach clear**: Limpar o stach

---

> git revert x git reset

**git reset HEAD~1**: Para resetar o HEAD voltando 1 passo, leva **hard** como padrão

**git reset --soft HEAD~1**: Move para index

**git reset --mixed HEAD~1**: Move para working directory

**git reset --hard HEAD~1**: Exclusão total

**git revert**: Gera um commit com as alterações inversas!

---

> git log

**git log**: Histórico cronológico de commits

**git log nome-da-pasta**: Ver histórico de pastas e arquivos específicos

**git log --oneline**: Resumo em uma linha

**git log --graph**: Histórico ilustrado

**gitk**: Mostra numa nova janela de forma um pouco mais gráfica

---

## Conceito de Flag (bandeiras):

Flags são atalhos ou aliases referência a um comando padrão para a realização de uma ação. Marcadas pelo traço + letra (EX: -a)

- **ls -a**: Mostrar arquivos ocultos

## Flags:

- **-b**: branch
- **-m**: message (mensagem)
- **-d**: delete (deletar)
- **-a**: all (todos)

---

## Significado:
**mv**: Mover

**echo >**: Criar arquivo

- **untracked** vai para **unstage**
- **unstage** é igual a **index**

**marge**: Juntas/Unir branches

**stach**: Caixa de alterações

**WIP**: Working-In-Progress

#### **VSC:**
- U: Untracked
- M: Modified

---

## Branches
**Definição**: galho/ramificação. É como uma nova pasta réplica da principal.

main e master: Nomes mais comuns para a branch principal

remote -v: ver o repositório online ao qual esse código está linkado

HEAD: aponta para o último commit válido e étambém (é você)! Vai apontar para onde você está localizado no espaço de branches

> Colocar nome descritivo para as branches!

> Usando vim:

**q** para sair

**:** para ir e apertar q

---

## Estrutura de título de commit

Imperativo!O que o commit faz? Simples e direto.

Corpo do commit: quebre em 75 char, adicione markdown, explique tudo

Vim é o editor de md do readme do commit do Git
Para sair de lá
:q! sair sem salvar

git config --global core.editor  "code --wait"
colocar um editor padrão para editar o readme

git config --global --unset core.editor
reverter a opção

git config --global core.editor  "vim"

Rodapé: 
Closes #1 para resolver um issue

ISERT para entrar no modo de edição
ESC para sair do mood de edição
:wq para salvar e sair

---

## Pull Request
Definição: Contribuir para projetos de outras pessoas, ou seja, um projeto que não é meu, eu não sou o usuário dono do projeto, quero contribuir, mas não tenho a permissão.

Mover o repositório de outra pessoa para o meu: Fork

Faz-se Pull Request através de um link ou no botão do GitHub

---

## Alias

Definir atalhos para comando:
git config --global alias.s status
git config --global --unset alias.s <- letra do alias definido anteriormente
git config --global --list: lista de configurações