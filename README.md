# Primeiros passos para desenvolver com o Angular
Esse projeto executa uma mensagem no navegador, aborda a interpolação e ensina como manipular arquivos com o Angular.

## Requisitos
- HTML básico.
- JavaScript básico.
- Node.js.
- Angular CLI.
- Visual Studio Code.

## Licença
Distribuido sob a licença MIT License. Veja `LICENSE` para mais informações.

## Comandos
Instale no node_modules:
>npm install

Para verificar se o Node.js está instalado:
>node -v 

Para verificar se o pacote do Node.js está instalado:
>npm -v

Instalar o Angular CLI no Linux:
>sudo npm install -g @angular/cli

Para verificar se o Angular CLI está instalado:
>ng version

O comando abaixo criou o projeto:
>ng new course-manager
- Não ativou as rotas
- Folha de estilo: CSS

## Entendendo os arquivos
- package.json: é onde adicionamos novas dependências.
- angular.json: contêm as informações globais e define qual arquivo vai inicializar a aplicação. (assets: contêm as imagens e arquivos estáticos, styles: contêm os estilos, scripts: contêm os scripts, index: é a página da aplicação, main: faz o bootstrap)
- node_modules: agrupa todas as dependências.
- app.module.ts: carrega o componente pai.

## Sobre o projeto
No app.component.ts adicionou o código:
>name: string = 'Fernanda Maki Hirose';

Para fazer o código acima aparecer no projeto adicionou a interpolação no app.component.html:
>{{ name }}

No app.component.ts criei um input código:
><input [ngModel]="name" name="name" >

Importei no app.module.ts:
>import { BrowserModule } from '@angular/platform-browser'; 

Por fim dentro do imports do app.module.ts adicionei:
>FormsModule

## Executar o projeto
>ng serve

## Digite no navegador para abrir o projeto
>http://localhost:4200/
