# formacao-angular-13

## Listar versões do nodejs:

Listar versões:
```
nvm list
```
Escolher versão
```
nvm use 18.20.4
```

## Downgrade do Node.js

Você pode instalar uma versão do Node.js que seja compatível com o Angular CLI 13.3.11. 

1. Verificar a compatibilidade<br>
- O Angular CLI 13.3.11 suporta o Node.js na faixa de versões LTS que estavam ativas na época. Geralmente, isso inclui versões do Node.js 14.x ou 16.x.
- Verifique a documentação oficial do Angular 13 para confirmar a compatibilidade, mas o Node.js 16.x é uma escolha segura.

2. Trocar para uma versão suportada do Node.js Se você estiver usando o nvm (Node Version Manager), pode instalar e usar uma versão compatível com o comando:
```
nvm install 16
nvm use 16
```
Caso não esteja usando o nvm, você pode baixar a versão específica do Node.js no site oficial: https://nodejs.org/.<br>

3. Verificar novamente Após instalar a versão correta do Node.js, execute novamente:
```
ng version
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
Isso retornará uma lista de todas as versões do framework Angular.

3. Ferramenta alternativa para explorar versões

Se a saída no terminal for muito longa, você pode instalar o pacote npm-check para visualizar pacotes e versões de forma interativa:
```
npm install -g npm-check
npm-check
```

## Trocar de versão do Angular

1. Trocar a versão do Angular CLI (Globalmente)

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
