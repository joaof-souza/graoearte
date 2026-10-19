☕ Grão & Arte - Torrefação e Café Especial

Este repositório contém o código-fonte do site institucional e catálogo de produtos da Grão & Arte, desenvolvido como parte da avaliação prática de desenvolvimento front-end.

📌 1. Visão Geral e Objetivo do Projeto

O objetivo principal deste projeto é simular uma entrega profissional de desenvolvimento front-end para o cliente fictício Grão & Arte - Torrefação e Café Especial. A aplicação foi projetada para conectar apreciadores de cafés especiais e microlotes a métodos de extração artesanais e planos de assinatura mensal.

A solução consiste em uma landing page responsiva e acessível que apresenta:

Banner principal com a proposta de valor da marca.

Catálogo de microlotes exclusivos em formato de cards.

Seção explicativa sobre o processo artesanal de torra.

Tabela comparativa dos planos do clube de assinatura.

Seção interativa de Perguntas Frequentes (FAQ).

Botão flutuante para contato direto via WhatsApp.

🛠️ 2. Tecnologias e Conceitos Aplicados

HTML5 Semântico: Estruturação orientada à acessibilidade e SEO, utilizando elementos adequados como <header>, <nav>, <main>, <section>, <article>, <details>, <summary> e <footer>.

CSS3 Moderno & Design System:

Variáveis CSS (:root): Padronização de tokens de design (paleta de cores, tipografia, sombras e espaçamentos).

Flexbox: Construção e alinhamento dos cards e layouts das seções.

Metodologia BEM (Block Element Modifier): Convenção de nomenclatura para manter o CSS modular e evitar conflitos de seletores.

Escala REM & Unidades Relativas: Definição da fonte base na raiz (html) e declaração de dimensões usando rem, %, vw e vh, restringindo o uso de px apenas a bordas e detalhes.

Google Fonts: Importação das famílias tipográficas Merriweather e Open Sans.

Design Responsivo: Aplicação de Media Queries para adaptação em smartphones, tablets e desktops.

Microinterações: Transições suaves (transition) e efeitos :hover em cards, botões e navegação.

📂 3. Organização da Arquitetura de Arquivos Adotada

O projeto adota uma estrita separação de responsabilidades, separando a estrutura semântica HTML da estilização CSS e dos recursos visuais:

grao-e-arte/
├── index.html          # Documento HTML5 semântico com todo o conteúdo da aplicação
├── css/
│   ├── variables.css   # Variáveis globais do Design System (Cores, fontes, sombras)
│   ├── reset.css       # Normalização de estilos padrão do navegador
│   └── style.css       # Estilização BEM, regras de layout e media queries para responsividade
├── assets/
│   └── images/         # Recursos visuais e imagens da aplicação
└── README.md           # Documentação oficial do projeto


🚀 4. Instruções de Visualização e Execução

Para rodar e visualizar o projeto localmente em sua máquina:

Clonar o Repositório:

git clone https://github.com/seu-usuario/seu-repositorio.git


Navegar até o diretório do projeto:

cd seu-repositorio


Executar a Aplicação:

Opção 1: Dê um duplo clique no arquivo index.html para abri-lo diretamente no navegador de sua preferência.

Opção 2: Se estiver utilizando o VS Code, clique com o botão direito sobre o arquivo index.html e selecione "Open with Live Server" para rodar em um servidor local com recarregamento automático.

💡 5. Principais Desafios Técnicos e Aprendizados

Gerenciamento de Posição Fixa (position: fixed):

Desafio: Trabalhar com o menu de navegação e o rodapé fixos simultaneamente exigiu cuidados para que o conteúdo principal (<main>) e o cabeçalho não se sobrepusessem.

Aprendizado: Implementação de compensação do topo (scroll-margin-top / padding-top) para garantir que os links âncora não cortassem o início dos títulos das seções durante a rolagem suave.

Aderência Rigorosa à Metodologia BEM:

Desafio: Manter a nomenclatura de classes coerente em seções repetitivas (como cards de catálogo e planos).

Aprendizado: Organização mental e do arquivo CSS em blocos independentes, o que facilitou a reusabilidade e manutenção do código.

Tipografia Fluida e Unidades Relativas (REM):

Desafio: Transitar do pensamento tradicional em pixels (px) para unidades relativas (rem e %).

Aprendizado: Compreensão prática do ajuste da fonte base na raiz e como isso melhora a acessibilidade do projeto para usuários que alteram o tamanho padrão de fonte do navegador.

Componentes Interativos sem JavaScript:

Desafio: Criar uma seção de FAQ funcional mantendo a aplicação leve.

Aprendizado: Utilização dos elementos semânticos nativos <details> e <summary> para criar acionadores colapsáveis nativos do HTML5.