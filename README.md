### Listar versões do nodejs:

Listar versões:
```
nvm list
```
Escolher versão
```
nvm use 18.20.4
```

### Downgrade do Node.js

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
### Outras configurações

- [Trabalhando com diferentes versões do Angular](https://www.alura.com.br/artigos/trabalhando-diferentes-versoes-angular?srsltid=AfmBOopbdRoB03f5PxXOult-9ChQkuKfoBA0MGNSnqeZFdb4TjX_SuSY)
- [Mudar versão do angular-cli](https://cursos.alura.com.br/forum/topico-mudar-versao-do-angula-cli-266813)
