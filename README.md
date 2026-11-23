<p align="center">
  <img src="assets/img/Logo-branca.png" alt="Logo MAREJAR" width="220" />
</p>

# MAREJAR Mobile — Planejamento Turístico e Experiências Locais no Litoral Norte de PE

Versão mobile do **MAREJAR**, desenvolvida no âmbito do Trabalho de Conclusão de Curso (TCC) apresentado ao Curso Técnico Integrado em Desenvolvimento de Sistemas da **Escola Técnica Estadual Jurandir Bezerra Lins** (2026), sob orientação do **Prof. Dr. Danilo Barbosa**.

A aplicação foca na experiência em dispositivos móveis para o **Litoral Norte de Pernambuco**, abrangendo **Igarassu, Goiana, Paulista, Olinda, Itapissuma e Ilha de Itamaracá**. A proposta reúne vivências, roteiros organizados por município, assistência por inteligência artificial (**MIA**), jornada gamificada (**Caça-maré**) e gestão de perfil em uma navegação adaptada para telas pequenas e empacotamento para Android.

## Funcionalidades Principais
- **Vitrine de destinos e vivências:** exploração na tela inicial com busca textual, filtros por categoria (Praias, História, Cultura e Gastronomia) e cards de pacotes/experiências com acesso aos roteiros.
- **Roteiros por município:** filtros por cidade (Olinda, Paulista, Igarassu, Itapissuma, Itamaracá e Goiana), detalhamento de paradas/dicas e salvamento local de roteiros.
- **Assistente MIA:** chat para solicitações de roteiros e dicas no litoral norte pernambucano, com atalhos rápidos e fallback local quando a API não está disponível.
- **Jornada e gamificação (Caça-maré):** acompanhamento de saldo e total de XP, metas de pontuação, conquistas por região, missões com envio de evidências (foto/vídeo), loja de recompensas com geração de código e histórico de atividades.
- **Perfil do usuário:** visualização e edição de dados cadastrais (nome, telefone, cidade e preferência no litoral), contagem de roteiros salvos e atalhos para a jornada.

## Tecnologias e Arquitetura
- **Front-end mobile:** HTML5 semântico, CSS3 (`global.css`, `components.css` e estilos por tela) e JavaScript (Vanilla JS), estruturado em layout mobile-first (`430px` de largura máxima em desktop com barra de navegação inferior em 5 abas).
- **Persistência local:** `localStorage` para dados de perfil (`marejar_user`), jornada/XP (`marejar_jornada_v1`) e roteiros salvos (`marejar_roteiros_salvos_v1`), permitindo uso contínuo inclusive sem conexão constante com o back-end.
- **Integração e publicação:** suporte a requisições `fetch` para endpoints da API (`http://localhost:3001`), publicação estática via **GitHub Pages** e empacotamento web-para-APK para testes em Android.

## Estrutura do Repositório
```text
marejar-mobile/
├── index.html          # Tela inicial de abertura
├── pages/
│   ├── login.html      # Acesso à conta
│   ├── cadastro.html   # Criação de conta
│   ├── home.html       # Vitrine, busca e filtros de vivências
│   ├── roteiros.html   # Roteiros por município e salvamento
│   ├── assistente.html # Chat com a assistente MIA
│   ├── guias.html      # Jornada e missões do Caça-maré
│   └── perfil.html     # Dados do explorador e edição
└── assets/
    ├── css/            # Estilos globais e componentes
    ├── js/             # Scripts auxiliares
    └── img/            # Logotipo e imagens das cidades/destinos

## Integrantes do Projeto
- Dante Vinícius Ferreira Lopes
- Gabrielly Chateaubriand Rosa
- João Enrick Silva Ferreira
- Juana Gabriela Gomes dos Santos
- Lázaro Filipe da Silva Borges
- Lívia Regina de Oliveira Pereira
- Luiz Guilherme da Silva Pereira
- Miguel Alves Dias de Moura
