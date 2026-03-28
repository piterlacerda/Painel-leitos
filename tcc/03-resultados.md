# 3. RESULTADOS

## 3.1 Indicadores Identificados na Literatura

A revisão de literatura permitiu identificar um conjunto de indicadores utilizados na gestão de leitos hospitalares. Os indicadores foram organizados em quatro dimensões: eficiência, qualidade, acesso e operacional.

### Quadro 1 — Indicadores de Gestão de Leitos por Dimensão

| Dimensão | Indicador | Definição | Fórmula | Meta de Referência |
|----------|-----------|-----------|---------|-------------------|
| **Eficiência** | Taxa de Ocupação | Percentual de leitos ocupados em relação ao total disponível | (Pacientes-dia / Leitos-dia) × 100 | 80-85% |
| Eficiência | Tempo Médio de Permanência (TMP) | Média de dias de internação | Total pacientes-dia / Nº de saídas | Varia por especialidade |
| Eficiência | Índice de Rotatividade | Pacientes atendidos por leito no período | Nº de saídas / Nº de leitos | 4-6 pacientes/leito/mês |
| Eficiência | Intervalo de Substituição | Tempo médio de leito vago entre internações | (Leitos-dia - Pacientes-dia) / Nº de saídas | < 1 dia |
| **Qualidade** | Taxa de Readmissão 30 dias | Pacientes readmitidos em até 30 dias | (Readmissões / Total de altas) × 100 | < 10% |
| Qualidade | Mortalidade Hospitalar | Óbitos em relação às saídas | (Óbitos / Total de saídas) × 100 | Varia por case-mix |
| **Acesso** | Tempo PS-Leito | Tempo da decisão de internar até ocupação | Mediana em horas | < 4 horas |
| **Operacional** | Leitos Bloqueados | Leitos indisponíveis por manutenção/limpeza | (Leitos bloqueados / Total) × 100 | < 5% |
| Operacional | Previsão de Altas | Pacientes com alta prevista nas próximas 24h | Contagem absoluta | — |

**Fonte:** Elaborado pelo autor com base em ANAHP (2022), AHRQ (2021) e revisão de literatura.

### 3.1.1 Indicadores de Eficiência

A **taxa de ocupação** foi o indicador mais citado na literatura, sendo considerado fundamental para avaliação da utilização dos recursos. Estudos apontam que taxas muito elevadas (acima de 90%) estão associadas a superlotação, aumento de eventos adversos e sobrecarga das equipes. Por outro lado, taxas muito baixas indicam ociosidade e desperdício de recursos (BITTENCOURT; HORTALE, 2009).

O **tempo médio de permanência (TMP)** permite identificar potenciais ineficiências no fluxo assistencial. Valores elevados podem indicar complicações clínicas, atrasos em exames ou procedimentos, dificuldades no planejamento da alta ou problemas sociais que impedem a liberação do paciente (DIAS, 2015).

O **índice de rotatividade** e o **intervalo de substituição** complementam a análise de eficiência, permitindo avaliar o giro de leitos e identificar gargalos no processo de preparação para novas admissões.

### 3.1.2 Indicadores de Qualidade

A **taxa de readmissão em 30 dias** é amplamente utilizada como indicador de qualidade da assistência e da segurança da alta hospitalar. Readmissões frequentes podem indicar alta precoce, falhas no planejamento de cuidados pós-alta ou inadequação do tratamento inicial (CMS, 2020).

A **mortalidade hospitalar** é indicador clássico de resultado, porém deve ser interpretada com cautela e ajustada pela gravidade dos casos (case-mix) para permitir comparações válidas.

### 3.1.3 Indicadores de Acesso

O **tempo entre PS e leito** reflete a eficiência do fluxo de internação e a capacidade de resposta do hospital à demanda. Tempos prolongados estão associados a pior prognóstico, especialmente em casos graves que necessitam de UTI (CHALFIN et al., 2007).

### 3.1.4 Indicadores Operacionais

O monitoramento de **leitos bloqueados** permite identificar perdas de capacidade por questões de manutenção, limpeza ou falta de equipe.

A **previsão de altas** é informação prospectiva fundamental para o planejamento de novas admissões e gestão do fluxo de pacientes.

## 3.2 Requisitos Funcionais do Sistema

A análise de requisitos identificou as funcionalidades essenciais para um sistema de monitoramento de leitos, organizadas por módulo.

### Quadro 2 — Requisitos Funcionais por Módulo

| Módulo | Funcionalidade | Prioridade |
|--------|----------------|------------|
| **Dashboard Principal** | Exibir taxa de ocupação geral em tempo real | Alta |
| Dashboard Principal | Mostrar número de leitos por status (ocupado/livre/bloqueado) | Alta |
| Dashboard Principal | Exibir TMP atual versus meta | Alta |
| Dashboard Principal | Mostrar previsão de altas (24h) | Alta |
| Dashboard Principal | Exibir alertas ativos | Alta |
| **Visão por Setor** | Listar setores com ocupação | Alta |
| Visão por Setor | Mostrar status individual de cada leito | Média |
| Visão por Setor | Identificar pacientes com alta prevista | Média |
| **Mapa de Leitos** | Visualização gráfica do layout | Média |
| Mapa de Leitos | Código de cores por status | Média |
| **Histórico** | Gráficos de tendência de ocupação | Média |
| Histórico | Comparativo entre períodos | Baixa |
| Histórico | Exportação de relatórios | Baixa |
| **Alertas** | Notificação de ocupação crítica (>90%) | Alta |
| Alertas | Alerta de leito parado (>24h) | Média |
| Alertas | Alerta de TMP acima da meta | Média |

**Fonte:** Elaborado pelo autor.

### 3.2.1 Perfis de Usuário

Foram identificados quatro perfis principais de usuários, com necessidades distintas de informação:

**Gestor de Leitos:** responsável operacional pela gestão diária, necessita de visão detalhada e alertas em tempo real para tomada de decisão imediata.

**Coordenador de Setor:** responsável por unidade específica (UTI, enfermaria, etc.), necessita de visão focada em seu setor com informações sobre previsão de altas e status dos leitos.

**Direção/Superintendência:** responsável pela gestão estratégica, necessita de indicadores consolidados e tendências para planejamento e avaliação de desempenho.

**Equipe Assistencial:** médicos e enfermeiros que necessitam consultar disponibilidade de leitos para solicitação de internações.

### 3.2.2 Regras de Alertas

O sistema de alertas foi estruturado com três níveis de prioridade:

| Nível | Situação | Condição | Ação Sugerida |
|-------|----------|----------|---------------|
| Crítico | Capacidade crítica | Ocupação > 90% | Acionar gestão, avaliar transferências |
| Atenção | Leito parado | Vago > 24h sem justificativa | Verificar disponibilidade para admissão |
| Atenção | Permanência elevada | TMP > meta do setor | Revisar casos, planejar altas |
| Informação | Previsão de alta | Alta prevista hoje | Preparar leito para nova admissão |

## 3.3 Arquitetura Funcional Proposta

A arquitetura funcional do painel foi organizada em cinco telas principais, conectadas por navegação intuitiva.

### Figura 1 — Estrutura de Navegação do Painel

```
┌─────────────────────────────────────────────────┐
│                    HEADER                        │
│  Logo | Título | Última atualização | Usuário   │
├─────────────────────────────────────────────────┤
│     Dashboard | Por Setor | Mapa | Histórico | Alertas    │
├─────────────────────────────────────────────────┤
│                                                  │
│              ÁREA DE CONTEÚDO                    │
│         (varia conforme tela selecionada)        │
│                                                  │
└─────────────────────────────────────────────────┘
```

### 3.3.1 Tela Dashboard Principal

A tela principal apresenta visão consolidada dos principais indicadores:

- **Cards de KPIs:** taxa de ocupação (com gauge visual), leitos disponíveis, TMP, previsão de altas
- **Tabela de setores:** ocupação por setor com barra de progresso e status
- **Lista de alertas:** alertas ativos ordenados por prioridade

### 3.3.2 Tela Visão por Setor

Permite visualização detalhada de cada unidade:

- **Seletor de setor:** botões para alternar entre setores
- **Grid de leitos:** visualização individual de cada leito com status (ocupado/livre/bloqueado)
- **Informações complementares:** tempo de ocupação, previsão de alta

### 3.3.3 Tela Mapa de Leitos

Apresenta visão consolidada de todos os leitos do hospital:

- **Grid visual:** representação gráfica de todos os leitos
- **Código de cores:** verde (livre), vermelho (ocupado), cinza (bloqueado)
- **Legenda:** explicação dos códigos visuais

### 3.3.4 Tela Histórico

Apresenta análise temporal dos indicadores:

- **Gráfico de tendência:** ocupação dos últimos 7 dias
- **Cards de indicadores mensais:** média de ocupação, rotatividade, intervalo de substituição, taxa de readmissão

### 3.3.5 Tela Alertas

Centraliza todos os alertas do sistema:

- **Lista completa:** todos os alertas com classificação por tipo
- **Filtros:** possibilidade de filtrar por prioridade ou tipo

## 3.4 Protótipo Desenvolvido

Foi desenvolvido protótipo funcional do painel de indicadores, disponível em: **https://painel-leitos.vercel.app**

### 3.4.1 Especificações Técnicas

- **Tecnologias:** HTML5, CSS3, JavaScript
- **Design responsivo:** adaptável a desktop, tablet e smartphone
- **Dados:** simulados para hospital de médio porte (97 leitos, 6 setores)

### 3.4.2 Características Implementadas

O protótipo implementa as seguintes funcionalidades:

1. **Dashboard com indicadores em tempo real:** gauge de ocupação, cards de KPIs, tabela de setores
2. **Navegação entre telas:** transições suaves entre as cinco visões principais
3. **Sistema de alertas visuais:** banner de alerta principal, lista de alertas com ícones e cores
4. **Visualização de leitos:** grid interativo com código de cores
5. **Dados de demonstração:** valores fictícios representativos de cenário hospitalar típico

### 3.4.3 Capturas de Tela

*(Inserir capturas de tela do protótipo no documento final)*

### Quadro 3 — Dados de Demonstração do Protótipo

| Setor | Leitos | Ocupados | Disponíveis | Bloqueados | Taxa de Ocupação |
|-------|--------|----------|-------------|------------|------------------|
| UTI Adulto | 10 | 9 | 1 | 0 | 90% |
| UTI Pediátrica | 6 | 4 | 2 | 0 | 67% |
| Enfermaria Clínica | 30 | 22 | 6 | 2 | 73% |
| Enfermaria Cirúrgica | 24 | 18 | 5 | 1 | 75% |
| Pediatria | 12 | 8 | 4 | 0 | 67% |
| Maternidade | 15 | 10 | 5 | 0 | 67% |
| **Total** | **97** | **71** | **23** | **3** | **73,2%** |

**Fonte:** Dados fictícios elaborados para demonstração do protótipo.

### 3.4.4 Paleta de Cores

A identidade visual do protótipo utilizou paleta moderna e profissional:

- **Primária:** #2563EB (azul vibrante) — elementos principais e ações
- **Sucesso/Disponível:** #10B981 (verde) — leitos livres, indicadores dentro da meta
- **Atenção:** #F59E0B (âmbar) — alertas de média prioridade
- **Crítico/Ocupado:** #EF4444 (vermelho) — alertas críticos, capacidade excedida
- **Neutro:** #6B7280 (cinza) — elementos desabilitados, leitos bloqueados

A escolha das cores seguiu princípios de acessibilidade e semântica visual, facilitando a interpretação rápida das informações pelos usuários.
