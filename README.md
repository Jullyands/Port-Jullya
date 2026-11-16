# Portfólio Profissional - Anna Jullya

**Aluna:** Anna Jullya Nascimento dos Santos  

## Descrição do Portfólio
Este projeto é um portfólio pessoal e acadêmico desenvolvido como evolução da atividade proposta no curso de Desenvolvimento de Sistemas da EADTEC. O site apresenta meu perfil profissional, minhas principais habilidades técnicas, projetos desenvolvidos em sala de aula e canais diretos para contato profissional.

## Tecnologias Utilizadas
* **HTML5:** Estruturação semântica das seções da página.
* **CSS3:** Personalização visual, tipografia (Google Fonts) e ajustes de layout.
* **Bootstrap 5.3:** Construção do grid responsivo, barra de navegação, carrossel de imagens, cartões e sistema de temas.
* **JavaScript:** Manipulação do DOM para alternância dinâmica de tema e ícones.
* **Devicon & SVG:** Ícones vetoriais das tecnologias e da interface.


## Funcionamento do Projeto
O site é estruturado em uma página única (*Single Page*) com navegação fluida por âncoras através do menu superior fixo (`#perfil`, `#projetos` e `#contato`). 
* **Início:** Exibe um carrossel interativo com imagens de projetos e códigos desenvolvidos.
* **Perfil:** Apresenta minhas informações acadêmicas, objetivo profissional e as ferramentas que domino.
* **Projetos:** Exibe cartões organizados com descrição e acesso aos meus trabalhos práticos em HTML e Python.
* **Contato:** Reúne botões de acesso rápido ao meu E-mail, GitHub e LinkedIn.

## Recurso Novo Adicionado
Foi implementado um **Alternador de Tema (Modo Claro / Modo Escuro)** diretamente na barra de navegação superior, permitindo que o visitante alterne a aparência visual de todo o site com um clique, acompanhado de mudança dinâmica entre os ícones de Lua e Sol.

## Como o Recurso foi Implementado
1. **Atributo de Tema do Bootstrap 5.3:** Foi adicionado o atributo `data-bs-theme="light"` na tag raiz `<html>` e utilizadas classes adaptáveis (`bg-body`, `text-muted`) para que os componentes respondam automaticamente à troca de tema.
2. **Estrutura do Botão e Ícones SVG:** Na barra de navegação, foi criado um botão (`#btnTema`) contendo dois elementos internos (`#iconeTema` e `#textoTema`) com ícones SVG embutidos.
3. **Lógica em JavaScript:** Foi adicionado um ouvinte de evento (`addEventListener('click')`) que verifica o valor atual de `data-bs-theme`. Quando está em `"light"`, o script altera para `"dark"`, substitui o SVG da lua pelo do sol, muda o texto para `"Modo Claro"` e ajusta a cor do botão; ao clicar novamente, reverte todas as alterações.
