# Formação Angular 13

## Configuração do Ambiente

Este guia detalha como configurar o ambiente necessário para trabalhar com o Angular CLI 13.0.4, incluindo a instalação do Node.js, NVM, Angular CLI, além de soluções para problemas comuns.

## 1. Instalando o Node.js

### Método 1: Instalação Direta

1. Acesse o site oficial do Node.js: https://nodejs.org.
   
2. Baixe a versão LTS (Long-Term Support) recomendada.
   
3. Execute o instalador e siga os passos:
    - Aceite os termos de licença.
    - Escolha as opções padrão.
    - Conclua a instalação.
  
4. Verifique a instalação:
```
node -v
npm -v
```
5. Atualize o npm (se necessário):
```
npm install -g npm
```
### Método 2: Gerenciamento de Versões com NVM

O NVM permite gerenciar várias versões do Node.js, ideal para projetos com diferentes requisitos.

1. Baixe o instalador do NVM:
    - Acesse: https://github.com/coreybutler/nvm-windows/releases.
    - Baixe e execute o arquivo `nvm-setup.exe`.
    - 
2. Instale o NVM seguindo as instruções do instalador.
   
3. Verifique a instalação:
```
nvm --version
```
**Usando o NVM**

1. Liste as versões disponíveis:
```
nvm list available
```
2. Instale a versão necessária:
```
nvm install 16.20.2
```
3. Ative a versão instalada:
```
nvm use 16.20.2
```
4. Verifique a versão ativa:
```
node -v
```
## 2. Instalando o Angular CLI

1. Instale o Angular CLI na versão desejada:
```
npm install -g @angular/cli@13.0.4
```
2. Verifique a instalação:
```
ng version
```
3. Confirme o caminho do executável:
```
where ng
```
## 3. Listando e Alterando Versões do Angular CLI
### 3.1 Listar Versões Disponíveis
- Listar todas as versões do Angular CLI:
```
npm view @angular/cli versions
```
- Verificar uma versão específica:
```
npm view @angular/cli@13.0.4 version
```
### 3.2 Alterar a Versão do Angular CLI
1. Desinstalar a versão atual:
```
npm uninstall -g @angular/cli
```
2. Instalar uma nova versão:
```
npm install -g @angular/cli@13.3.11
```
3. Verificar a versão instalada:
```
ng version
```
## 4. Solução de Problemas
### 4.1 Reinstalar o Node.js e o Angular CLI

Se problemas persistirem, reinstale o Node.js e o Angular CLI:

1. Desinstale o Node.js e exclua as pastas residuais:
```
C:\Program Files\nodejs
C:\Users\<User>\AppData\Roaming\npm
C:\Users\<User>\AppData\Roaming\npm-cache
```
2. Reinstale o Node.js com o NVM.
3. Reinstale o Angular CLI:
```
npm install -g @angular/cli@13.0.4
```
### 4.2 Recriar Arquivos do Angular CLI
Se os executáveis `ng`, `ng.cmd` ou `ng.ps1` estiverem ausentes:
1. Navegue até o diretório:
```
C:\Users\<User>\AppData\Roaming\npm
```
2. Crie os arquivos necessários:

**Arquivo** `ng.cmd`
- Conteúdo:
```
@echo off
node "%~dp0\node_modules\@angular\cli\bin\ng.js" %*
```
**Arquivo** `ng.ps1`
- Conteúdo:
```
node "$PSScriptRoot\node_modules\@angular\cli\bin\ng.js" $args
```
**Arquivo** `ng`
- Conteúdo:
```
#!/bin/sh
node "$(dirname "$0")/node_modules/@angular/cli/bin/ng.js" "$@"
```






### Outras configurações

- [Trabalhando com diferentes versões do Angular](https://www.alura.com.br/artigos/trabalhando-diferentes-versoes-angular?srsltid=AfmBOopbdRoB03f5PxXOult-9ChQkuKfoBA0MGNSnqeZFdb4TjX_SuSY)
- [Mudar versão do angular-cli](https://cursos.alura.com.br/forum/topico-mudar-versao-do-angula-cli-266813)
