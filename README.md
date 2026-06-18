#  Landing Page e RSVP Inteligente com Supabase

Uma Single Page Application (SPA) moderna e responsiva desenvolvida para gerenciar convites digitais, confirmações de presença (RSVP) em tempo real e centralizar contribuições voluntárias.

##  Sobre o Projeto
Esta aplicação foi projetada para modernizar a experiência de convites para eventos. O grande diferencial técnico é a adoção de uma arquitetura *Serverless* e *BaaS (Backend as a Service)*. A aplicação se comunica diretamente do front-end com um banco de dados PostgreSQL hospedado no Supabase, garantindo armazenamento estruturado e instantâneo sem a necessidade de instanciar e gerenciar um servidor backend intermediário.

A segurança da comunicação direta é garantida pelas políticas de RLS (*Row Level Security*) do PostgreSQL, permitindo que a chave anônima pública seja utilizada de forma segura em ambiente estático (GitHub Pages).

## 🛠️ Tecnologias e Ferramentas
* **Front-end:** HTML5 semântico e Tailwind CSS (via CDN) com foco em responsividade *Mobile-First*.
* **Lógica / DOM:** JavaScript Vanilla (manipulação de formulários, validação, Intersection Observer para animações de *scroll reveal* e Clipboard API para interação do usuário).
* **Banco de Dados:** Supabase / PostgreSQL (gerenciamento de tabelas, políticas RLS e integração via módulo ESM `@supabase/supabase-js`).
* **Hospedagem:** GitHub Pages.

##  Principais Funcionalidades
* **RSVP Assíncrono:** Formulário dinâmico que envia dados ao PostgreSQL utilizando *Fetch API/Promises*, provendo feedback visual imediato de "loading" e "sucesso" sem recarregar a página.
* **Módulo Financeiro Integrado:** Área dedicada a contribuições via Pix, com funcionalidade "Copiar e Colar" nativa para melhorar a experiência do usuário (UX).
* **Scroll Reveal Customizado:** Elementos visuais que reagem à posição da rolagem da página (Intersection Observer), aumentando a percepção de valor do design da interface.
