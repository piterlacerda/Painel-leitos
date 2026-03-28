# 2. METODOLOGIA

## 2.1 Tipo de Estudo

Trata-se de uma pesquisa aplicada, de natureza descritiva e exploratória, com abordagem qualitativa.

A pesquisa é classificada como **aplicada** por ter como objetivo gerar conhecimento para aplicação prática, direcionado à solução de um problema específico — a gestão de leitos hospitalares (GIL, 2019).

É **descritiva** por buscar caracterizar os indicadores e requisitos para sistemas de monitoramento de leitos, estabelecendo relações entre variáveis sem manipulação experimental (MARCONI; LAKATOS, 2017).

É **exploratória** por investigar um tema ainda pouco sistematizado no contexto brasileiro, buscando proporcionar maior familiaridade com o problema e construir hipóteses para estudos futuros (GIL, 2019).

A abordagem **qualitativa** foi escolhida por permitir a análise aprofundada de conceitos, requisitos e funcionalidades, com foco na compreensão do fenômeno estudado em sua complexidade (MINAYO, 2014).

## 2.2 Procedimentos Metodológicos

O desenvolvimento deste trabalho seguiu quatro etapas sequenciais e complementares:

### 2.2.1 Etapa 1 — Revisão de Literatura

Realizou-se revisão de literatura do tipo narrativa, com o objetivo de identificar os principais indicadores de gestão de leitos hospitalares e as evidências sobre a efetividade de dashboards na gestão hospitalar.

**Bases de dados consultadas:**
- PubMed/MEDLINE
- Biblioteca Virtual em Saúde (BVS)
- Scientific Electronic Library Online (SciELO)
- Google Scholar

**Descritores utilizados:**
- Em português: "gestão de leitos", "indicadores hospitalares", "painel de indicadores", "dashboard hospitalar", "sistemas de informação em saúde"
- Em inglês: "hospital bed management", "bed occupancy indicators", "healthcare dashboard", "bed management system", "hospital information systems"

**Critérios de inclusão:**
- Artigos publicados em português, inglês ou espanhol
- Publicações dos últimos 10 anos (2014-2024)
- Estudos que abordassem indicadores de gestão de leitos e/ou dashboards em contexto hospitalar
- Acesso ao texto completo disponível

**Critérios de exclusão:**
- Editoriais, cartas ao editor e resumos de congressos
- Estudos focados exclusivamente em aspectos clínicos sem relação com gestão
- Publicações duplicadas

A busca foi complementada por análise de documentos técnicos de entidades de referência como:
- Associação Nacional de Hospitais Privados (ANAHP) — Observatório ANAHP
- Organização Nacional de Acreditação (ONA)
- Agency for Healthcare Research and Quality (AHRQ)
- Joint Commission International (JCI)
- Ministério da Saúde do Brasil

### 2.2.2 Etapa 2 — Análise de Requisitos

Com base na revisão de literatura e nos documentos técnicos analisados, foram definidos os requisitos funcionais para um sistema de monitoramento de leitos.

A análise de requisitos seguiu metodologia adaptada de engenharia de software, incluindo:

**Identificação de usuários:** definição dos perfis de usuários do sistema e suas necessidades específicas de informação.

**Levantamento de funcionalidades:** listagem das funcionalidades essenciais para atender às necessidades identificadas.

**Especificação de indicadores:** seleção e definição operacional dos indicadores a serem monitorados, incluindo fórmulas de cálculo, periodicidade e metas de referência.

**Definição de alertas:** estabelecimento de critérios para geração de alertas automáticos com base em limites predefinidos.

### 2.2.3 Etapa 3 — Proposição da Arquitetura Funcional

A partir dos requisitos levantados, foi proposta a arquitetura funcional do painel de indicadores, incluindo:

- Estrutura de telas e navegação
- Hierarquia de informações
- Elementos visuais (gráficos, tabelas, indicadores)
- Fluxo de interação do usuário
- Integrações necessárias com sistemas hospitalares

A arquitetura foi documentada por meio de diagramas de fluxo e especificações funcionais.

### 2.2.4 Etapa 4 — Prototipagem

Foi desenvolvido um protótipo funcional do painel de indicadores, utilizando tecnologias web (HTML, CSS, JavaScript) para permitir visualização e interação com a solução proposta.

O protótipo foi construído com dados fictícios representativos de um hospital de médio porte, permitindo demonstrar as funcionalidades planejadas e validar a proposta conceitual.

**Características técnicas do protótipo:**
- Interface responsiva (adaptável a diferentes dispositivos)
- Navegação entre diferentes visões (dashboard, setores, mapa de leitos, histórico, alertas)
- Visualização de indicadores com código de cores
- Simulação de dados em tempo real
- Elementos interativos para exploração dos dados

## 2.3 Análise de Dados

A análise dos dados coletados na revisão de literatura seguiu os princípios da análise de conteúdo temática (BARDIN, 2016), compreendendo:

**Pré-análise:** leitura flutuante dos materiais selecionados para familiarização com o conteúdo.

**Exploração do material:** identificação e codificação das unidades de análise relacionadas a indicadores de gestão de leitos, requisitos de sistemas e evidências de efetividade.

**Tratamento dos resultados:** síntese narrativa dos achados, categorização dos indicadores por dimensão (eficiência, qualidade, acesso, operacional) e consolidação dos requisitos funcionais.

Os indicadores identificados foram organizados em matriz contendo: nome do indicador, definição operacional, fórmula de cálculo, periodicidade recomendada, meta de referência e fonte.

## 2.4 Aspectos Éticos

Por tratar-se de pesquisa bibliográfica e proposta conceitual, sem coleta de dados primários com seres humanos, o estudo dispensa apreciação por Comitê de Ética em Pesquisa, conforme Resolução CNS nº 510/2016 (BRASIL, 2016).

O protótipo desenvolvido utiliza exclusivamente dados fictícios, sem qualquer referência a informações reais de pacientes ou instituições de saúde.

Todas as fontes consultadas foram devidamente referenciadas, em conformidade com as normas da Associação Brasileira de Normas Técnicas (ABNT).

## 2.5 Limitações Metodológicas

Este estudo apresenta limitações que devem ser consideradas na interpretação dos resultados:

1. **Revisão narrativa:** por não se tratar de revisão sistemática, a seleção dos estudos pode estar sujeita a viés de seleção.

2. **Proposta conceitual:** o painel desenvolvido é um protótipo conceitual, não tendo sido implementado ou testado em ambiente real de produção.

3. **Dados simulados:** a ausência de dados reais limita a avaliação da aplicabilidade prática e dos potenciais impactos da solução.

4. **Contexto específico:** as recomendações podem necessitar de adaptações para aplicação em diferentes contextos institucionais (porte, natureza jurídica, perfil assistencial).

Essas limitações apontam para a necessidade de estudos futuros que implementem e avaliem a solução proposta em ambientes hospitalares reais.

---

## Referências (parciais - seção Metodologia)

BARDIN, L. Análise de Conteúdo. São Paulo: Edições 70, 2016.

BRASIL. Conselho Nacional de Saúde. Resolução nº 510, de 07 de abril de 2016. Dispõe sobre as normas aplicáveis a pesquisas em Ciências Humanas e Sociais. Diário Oficial da União, Brasília, 2016.

GIL, A. C. Métodos e técnicas de pesquisa social. 7. ed. São Paulo: Atlas, 2019.

MARCONI, M. A.; LAKATOS, E. M. Fundamentos de metodologia científica. 8. ed. São Paulo: Atlas, 2017.

MINAYO, M. C. S. O desafio do conhecimento: pesquisa qualitativa em saúde. 14. ed. São Paulo: Hucitec, 2014.
