# formacao-angular-13

## Versões do nodejs:

Instalar uma versão:
```
nvm install 7.8.0
```
Listar versões:
```
nvm list
```
Escolher versão
```
nvm use 7.8.0
```

## Versões disponíveis do Angular CLI

1. Listar todas as versões disponíveis do Angular CLI

Você pode usar o comando abaixo para listar todas as versões publicadas no npm para o Angular CLI:
```
npm view @angular/cli versions
```
Esse comando retornará uma lista de todas as versões publicadas.

2. Listar todas as versões disponíveis do Angular Framework

Para verificar as versões disponíveis de outros pacotes do Angular, como @angular/core, use:
```
npm view @angular/core versions
```
Isso retornará uma lista de todas as versões do framework Angular.<br>

Use este comando para verificar especificamente pela versão desejada:
```
npm view @angular/cli@13.0.4 version
```
3. Ferramenta alternativa para explorar versões

Se a saída no terminal for muito longa, você pode instalar o pacote npm-check para visualizar pacotes e versões de forma interativa:
```
npm install -g npm-check
npm-check
```

## Trocar de versão do Angular

Se você deseja trocar a versão do Angular CLI instalada globalmente:

a) Desinstalar a versão atual

Desinstale a versão atual do Angular CLI:
```
npm uninstall -g @angular/cli
```
b) Instalar a versão desejada

Instale a versão específica que você deseja (por exemplo, 13.3.11):
```
npm install -g @angular/cli@13.3.11
```
c) Verificar a versão instalada

Após a instalação, confirme que a nova versão está ativa:
```
ng version
```
### Outras configurações

- [Trabalhando com diferentes versões do Angular](https://www.alura.com.br/artigos/trabalhando-diferentes-versoes-angular?srsltid=AfmBOopbdRoB03f5PxXOult-9ChQkuKfoBA0MGNSnqeZFdb4TjX_SuSY)
- [Mudar versão do angular-cli](https://cursos.alura.com.br/forum/topico-mudar-versao-do-angula-cli-266813)
