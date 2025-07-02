# Documento de Implementação: Website de Psicologia Focado em TEA no Brasil

Este documento serve como um guia técnico e estratégico para agentes de IA e desenvolvedores que trabalham na criação e manutenção do website para uma prática de psicologia especializada em Transtorno do Espectro Autista (TEA) no Brasil. Ele é derivado e resume as diretrizes do `AGENTS.md` original, focando nos aspectos de implementação.

## Seção 1: Infraestrutura Técnica e de Hospedagem

**Objetivo:** Garantir desempenho, segurança e escalabilidade.

### 1.1 Hospedagem e Domínio
- **Provedor Recomendado:** Hostinger (servidores no Brasil).
- **Plano:** "WordPress" ou "Business" de longo prazo.
- **Data Center:** Localizado no Brasil.
- **Alternativa:** KingHost.
- **Ação:** Adquirir plano na Hostinger.com.br, selecionar data center no Brasil, ativar renovação automática.

### 1.2 Configuração do WordPress e Plugins Essenciais
- **CMS:** WordPress.
- **Plugins Essenciais:**
    - **Construtor de Páginas:** Elementor Pro (para layouts neuro-inclusivos).
        - Configuração: Usar configurações globais de cores/fontes, criar templates.
    - **SEO:** Rank Math SEO (SEO local, schema médico).
        - Configuração: Ativar módulo SEO Local, configurar schema `MedicalBusiness`, `Physician`, `Article`.
    - **Desempenho/Cache:** WP Rocket (cache, minificação, lazy loading).
        - Configuração: Ativar cache de página, minificação CSS/JS, lazy loading.
    - **Segurança:** Wordfence Security ou Sucuri Security (proteção contra ameaças).
        - Configuração: Ativar WAF, scans regulares, autenticação de dois fatores.
    - **Formulários:** WPForms ou Elementor Pro Forms (formulários acessíveis).
        - Configuração: Labels visíveis, evitar placeholder como label, anti-spam.
    - **Análise de Dados:** MonsterInsights (integração Google Analytics 4).
        - Configuração: Conectar GA4, rastrear eventos.
    - **Auditoria de Acessibilidade (Desenvolvimento):** WAVE Web Accessibility Evaluation Tool.

## Seção 2: SEO e Aquisição de Pacientes

**Objetivo:** Aumentar a visibilidade para o público-alvo (pais, cuidadores, indivíduos buscando serviços para TEA).

### 2.1 Otimização do Perfil da Empresa no Google (Google Business Profile - GBP)
- **Importância:** Principal ativo digital local.
- **Diretrizes:**
    1. Criação e Verificação (`google.com/business`, nome e endereço exatos).
    2. Preenchimento Completo (nome, endereço, telefone, site, horários, descrição).
    3. Seleção de Categoria (Primária: "Psicólogo" / "Clínica de Psicologia"; Secundárias relevantes).
    4. Descrição dos Serviços (detalhar especializações, palavras-chave: "terapia para autismo", "ABA", "TCC para TEA", termos geográficos).
    5. Fotografias de Alta Qualidade (exterior, recepção, salas).
    6. Gestão de Avaliações (incentivar e responder a todas profissionalmente).
    7. Utilização do Google Posts (atualizações do blog, notícias).
    8. Seção de Perguntas e Respostas (Q&A) (popular com perguntas comuns).

### 2.2 Estrutura Abrangente de SEO no Website
- **SEO On-Page:**
    - Integração de Palavras-chave (H1, meta título/descrição, URL, conteúdo).
    - Linkagem Interna (conectar páginas e posts de blog).
- **SEO Técnico:**
    - Marcação de Schema (Dados Estruturados: `MedicalBusiness`, `Physician`, `Article`).
    - Design Responsivo (Mobile-First).
    - Velocidade do Site (Core Web Vitals).
- **SEO Off-Page:**
    - Citações Locais (NAP consistente em diretórios relevantes).

### 2.3 Conteúdo Hiperlocal e Estratégia de Geotargeting
- **Objetivo:** Estabelecer autoridade local em TEA.
- **Implementação:**
    - Páginas de Serviço com Localização (ex: "Terapia ABA em Diadema").
    - Conteúdo de Blog com Foco Local (ex: "Recursos de Apoio para Famílias com Crianças Autistas em Diadema").

## Seção 3: Arquitetura da Informação e Conteúdo Empático

**Objetivo:** Criar um ecossistema de informação empático, autoritativo e valioso, otimizado para SEO e focado no usuário.

### 3.1 Arquitetura Central do Website (Sitemap)
- **Navegação:** Simples, previsível, lógica.
- **Páginas Principais:**
    - **Início (Home):** (`index.html`) Quem é, especialização (TEA), a quem ajuda. Imagem calma, proposta de valor, intro serviços, bio psicólogo, CTA.
    - **Sobre [Nome do Psicólogo(a)]:** (`sobre.html`) Biografia profissional, foto, credenciais (CRP), formação, filosofia.
    - **Serviços:** (`servicos/index.html`) Página mãe, introduz e linka para páginas de serviços detalhadas.
        - **Terapia ABA:** (`servicos/terapia-aba.html`) O que é, benefícios, estrutura.
        - **TCC para TEA:** (`servicos/terapia-cognitivo-comportamental.html`) Adaptação para adolescentes/adultos com TEA.
        - **Orientação para Pais:** (`servicos/orientacao-pais.html`) Apoio e estratégias.
    - **Blog / Recursos:** (`blog/index.html`) Hub de conteúdo educativo, navegável.
    - **Contato:** (`contato.html`) Endereço, mapa Google, telefone clicável, formulário, horários.

### 3.2 Blueprint do Conteúdo Educativo
- **Missão:** Posicionar como recurso local confiável sobre TEA.
- **Estratégia:** Conteúdo Pilar (guias longos) e posts satélite (clusters).
- **Clusters de Conteúdo Identificados:**
    1. Diagnóstico Precoce e Sinais.
    2. Intervenções Terapêuticas.
    3. Orientação Parental e Estratégias para Casa.
    4. Inclusão Escolar e Social.

### 3.3 Léxico de Palavras-chave Semânticas
- **Organização:** Por intenção do usuário.
- **Categorias de Intenção:**
    - **Informacional ("Quero saber"):** Posts de blog, guias, FAQs (ex: "sinais de autismo em bebês").
    - **Navegacional ("Quero ir para"):** Nome da marca (ex: "[Nome da Clínica] psicologia").
    - **Transacional/Comercial ("Quero fazer/contratar"):** Páginas de serviço, contato (ex: "psicólogo especialista em autismo em Diadema").

## Seção 4: Experiência do Usuário (UX/UI) Neuro-Inclusiva e Terapêutica

**Objetivo:** Criar um espaço digital calmante, confiável e acessível, especialmente para usuários neurodivergentes.

### 4.1 Princípios Fundamentais do Design Neuro-Inclusivo (Alinhado com WCAG)
- **Ambiente:** "Baixo estímulo" (low-arousal), minimizar carga cognitiva, evitar sobrecarga sensorial.
- **Diretrizes Chave:**
    1. **Reduzir Sobrecarga Sensorial:**
        - Sem mídia de reprodução automática.
        - Evitar elementos brilhantes/piscantes, animações rápidas, cores excessivas. Animações subtis.
        - Espaço em branco generoso.
    2. **Garantir Previsibilidade e Consistência:**
        - Navegação e layout consistentes.
        - Estrutura clara (cabeçalhos H1-H3).
        - Links e botões descritivos.
    3. **Melhorar Legibilidade e Compreensibilidade:**
        - Linguagem simples e direta.
        - Texto legível (alinhado à esquerda, comprimento de linha 50-75 caracteres).
        - Alto Contraste (mínimo WCAG AA 4.5:1).

### 4.2 Sistema de Identidade Visual: Paleta Terapêutica e Tipografia
- **Objetivo:** Evocar calma, confiança, profissionalismo.
- **Paleta de Cores Prescrita (HEX):**
    - **Primária (Confiança/Calma):** Azul suave/dessaturado (ex: `#6A8EAE` ou `#A2B9D1`).
    - **Secundária (Saúde/Crescimento):** Verde suave/natural (ex: `#B2C2A5`).
    - **Acento (Ação/Atenção):** Coral suave ou terracota (ex: `#E57F84`) - uso moderado para CTAs.
    - **Cor do Texto:** Cinzento escuro (ex: `#333333`).
    - **Fundo:** Branco ou cinzento muito claro (ex: `#FFFFFF` ou `#F4F4F4`).
- **Sistema de Tipografia (Google Fonts):**
    - **Cabeçalhos:** Montserrat (geométrica, limpa, versátil).
    - **Corpo do Texto:** Roboto ou Open Sans (alta legibilidade, neutras, amigáveis).
    - **Tamanho da Fonte:** Mínimo 16px para corpo, unidades relativas (em/rem), espaçamento entre linhas generoso (ex: 1.5).

### 4.3 Layout, Navegação e Design de Interação
- **Layout:** Coluna única para conteúdo principal na maioria das páginas. Grelha simples para consistência.
- **Navegação:** Menu principal simples (5-7 itens). Evitar menus suspensos complexos; se necessários, devem ser acessíveis por teclado.
- **Formulários:**
    - Labels claras e sempre visíveis (acima do campo).
    - Não usar apenas placeholder text.
    - Instruções claras, mensagens de erro úteis.
    - Dividir formulários longos em etapas.

## Conclusões e Recomendações Finais

Este documento visa guiar a implementação de um website que seja:
1.  **Tecnicamente Confiável:** Base sólida de hospedagem, velocidade e segurança.
2.  **Altamente Visível:** Estratégia de SEO robusta (GBP, conteúdo hiperlocal).
3.  **Empaticamente Informativo:** Conteúdo que constrói confiança e demonstra autoridade (E-E-A-T).
4.  **Terapeuticamente Desenhado:** Design neuro-inclusivo, calmo e acessível.

A implementação rigorosa destas diretrizes resultará em um ativo digital valioso para a prática e para a comunidade TEA.
