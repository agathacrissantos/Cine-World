# Documentação de Requisitos e Regras de Negócios

## 1. Introdução
**Objetivo do Documento:** Este documento detalha os requisitos funcionais e não funcionais, bem como as regras de negócios para o desenvolvimento do site de filmes "CineWorld".

## 2. Requisitos Funcionais
**2.1. Sistema de Cadastro e Login**
- **Descrição:** Usuários devem poder se cadastrar e fazer login no site.
- **Funcionalidades:**
  - Campo de e-mail obrigatório.
  - Campo de senha com no mínimo 8 caracteres.
  - Opção de recuperação de senha via e-mail.
  - Autenticação via redes sociais (Google, Facebook).

**2.2. Catálogo de Filmes**
- **Descrição:** O site deve exibir uma lista de filmes disponíveis.
- **Funcionalidades:**
  - Exibição de filmes por gênero, lançamento, popularidade.
  - Busca por nome, diretor, elenco, e ano.
  - Filtros por gênero, avaliação, data de lançamento.
  - Páginas de detalhes dos filmes com sinopse, trailer, elenco, e críticas.

**2.3. Avaliação e Comentários**
- **Descrição:** Usuários devem poder avaliar e comentar sobre filmes.
- **Funcionalidades:**
  - Sistema de avaliação com estrelas (1 a 5).
  - Campo de comentário.
  - Moderação de comentários para garantir conteúdo apropriado.

**2.4. Críticas e Artigos**
- **Descrição:** O site deve permitir a publicação de críticas e artigos sobre filmes.
- **Funcionalidades:**
  - Sistema de submissão de críticas e artigos.
  - Revisão e aprovação de conteúdos por editores.
  - Exibição de críticas e artigos na página de detalhes dos filmes.

## 3. Requisitos Não Funcionais
**3.1. Desempenho**
- **Descrição:** O site deve ter um tempo de carregamento inferior a 3 segundos.
- **Funcionalidades:**
  - Otimização de imagens e recursos.
  - Uso de CDN para distribuição de conteúdo.

**3.2. Segurança**
- **Descrição:** O site deve garantir a segurança dos dados dos usuários.
- **Funcionalidades:**
  - Criptografia de dados sensíveis.
  - Certificação SSL.
  - Medidas contra ataques DDoS.

## 4. Regras de Negócios

**4.1. Política de Avaliação**
- **Regra:** Usuários só podem avaliar um filme uma vez.
- **Descrição:** Cada usuário pode dar uma avaliação por filme, podendo editar a avaliação posteriormente.
- **Exemplo:**
  - Usuário avalia um filme com 4 estrelas -> Pode editar para 5 estrelas, mas não pode adicionar uma nova avaliação.

**4.2. Moderação de Comentários**
- **Regra:** Comentários inadequados devem ser removidos.
- **Descrição:** Comentários contendo linguagem ofensiva, spam ou conteúdo impróprio serão removidos pelos moderadores.
- **Exemplo:**
  - Comentário com linguagem ofensiva -> Removido por moderador.

**4.3. Publicação de Críticas**
- **Regra:** Críticas devem ser aprovadas por um editor antes da publicação.
- **Descrição:** Críticas submetidas pelos usuários serão revisadas por um editor para garantir qualidade e conformidade com as políticas do site.
- **Exemplo:**
  - Usuário submete crítica -> Editor revisa e aprova -> Crítica publicada.

## 5. Fluxos de Trabalho

**5.1. Fluxo de Cadastro e Login**
1. Usuário acessa a página de cadastro/login.
2. Preenche os campos obrigatórios (e-mail e senha).
3. (Para cadastro) Recebe e-mail de confirmação e clica no link.
4. (Para login) Acesso concedido após validação das credenciais.

**5.2. Fluxo de Avaliação de Filme**
1. Usuário acessa a página de detalhes do filme.
2. Seleciona a quantidade de estrelas para avaliar.
3. (Opcional) Adiciona um comentário sobre o filme.
4. Submete a avaliação.
5. Avaliação é exibida na página de detalhes do filme.

**5.3. Fluxo de Submissão de Crítica**
1. Usuário acessa a página de submissão de crítica.
2. Preenche o formulário com título, conteúdo e classificação do filme.
3. Submete a crítica.
4. Editor revisa e aprova a crítica.
5. Crítica aprovada é exibida na página de detalhes do filme.
