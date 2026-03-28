# Requisitos Funcionais - Painel de Gestão de Leitos

## 1. Perfis de Usuário

| Perfil | Descrição | Funcionalidades |
|--------|-----------|-----------------|
| Gestor de Leitos | Responsável operacional pela gestão de leitos | Visão completa, alertas, ações |
| Coordenador de Setor | Responsável por unidade específica | Visão do setor, previsão de altas |
| Direção/Superintendência | Gestão estratégica | Indicadores consolidados, tendências |
| Equipe Assistencial | Médicos, enfermeiros | Consulta de disponibilidade |

---

## 2. Módulos do Sistema

### 2.1 Dashboard Principal
**Funcionalidades:**
- [ ] Exibir taxa de ocupação geral em tempo real
- [ ] Mostrar número de leitos disponíveis/ocupados/bloqueados
- [ ] Exibir tempo médio de permanência atual vs. meta
- [ ] Mostrar previsão de altas nas próximas 24h
- [ ] Exibir alertas ativos (críticos, atenção)
- [ ] Permitir filtro por período (hoje, semana, mês)

**Indicadores visuais:**
- Gauge de ocupação (com cores por faixa)
- Cards com números principais
- Mini-gráficos de tendência (sparklines)

### 2.2 Visão por Setor
**Funcionalidades:**
- [ ] Listar setores/unidades (UTI, Enfermaria, Pediatria, etc.)
- [ ] Exibir ocupação por setor
- [ ] Mostrar lista de leitos com status (ocupado/livre/bloqueado)
- [ ] Exibir tempo de ocupação atual de cada leito
- [ ] Identificar pacientes com alta prevista
- [ ] Filtrar por tipo de leito (adulto, pediátrico, isolamento)

**Alertas por setor:**
- Ocupação crítica (> 90%)
- Leito vago há mais de 24h
- Permanência acima da meta

### 2.3 Mapa de Leitos
**Funcionalidades:**
- [ ] Visualização gráfica do layout de leitos
- [ ] Código de cores por status
- [ ] Clique para ver detalhes do leito/paciente
- [ ] Identificação visual de isolamentos

### 2.4 Indicadores Históricos
**Funcionalidades:**
- [ ] Gráfico de ocupação ao longo do tempo
- [ ] Gráfico de TMP por mês
- [ ] Gráfico de rotatividade
- [ ] Comparativo entre setores
- [ ] Exportação de dados (CSV, PDF)

### 2.5 Sistema de Alertas
**Tipos de alerta:**
| Tipo | Condição | Prioridade |
|------|----------|------------|
| Capacidade crítica | Ocupação > 90% | Alta |
| Leito parado | Vago > 24h sem justificativa | Média |
| Permanência elevada | TMP > meta do setor | Média |
| Previsão de alta | Alta prevista hoje | Info |
| Ociosidade | Ocupação < 60% | Baixa |

**Funcionalidades:**
- [ ] Notificação visual no painel
- [ ] Histórico de alertas
- [ ] Filtro por tipo e prioridade

### 2.6 Relatórios
**Funcionalidades:**
- [ ] Relatório diário de ocupação
- [ ] Relatório mensal de indicadores
- [ ] Relatório comparativo (mês atual vs. anterior)
- [ ] Exportação em PDF

---

## 3. Requisitos Não-Funcionais

### 3.1 Usabilidade
- Interface intuitiva e responsiva
- Visualização clara em monitores grandes (NOC) e tablets
- Tempo de carregamento < 3 segundos
- Acessibilidade (contraste, tamanho de fonte)

### 3.2 Performance
- Atualização de dados em tempo real (ou intervalo configurável)
- Suporte a múltiplos usuários simultâneos

### 3.3 Segurança
- Autenticação de usuários
- Controle de acesso por perfil
- Log de acessos

### 3.4 Integração
- API para integração com sistemas hospitalares (HIS)
- Possibilidade de integração com e-SUS/CNES
- Importação de dados via arquivo (CSV)

---

## 4. Fluxo de Telas (Wireframe)

```
[Login] 
    ↓
[Dashboard Principal]
    ├── [Visão por Setor]
    │       └── [Detalhes do Leito]
    ├── [Mapa de Leitos]
    ├── [Indicadores Históricos]
    ├── [Alertas]
    └── [Relatórios]
```

---

## 5. Paleta de Cores e Design

### Cores principais
- **Primária:** #2563EB (azul vibrante)
- **Sucesso/Disponível:** #10B981 (verde)
- **Atenção:** #F59E0B (âmbar)
- **Crítico/Ocupado:** #EF4444 (vermelho)
- **Neutro/Bloqueado:** #6B7280 (cinza)

### Background
- Fundo geral: #F8FAFC
- Cards: #FFFFFF
- Texto principal: #1E293B
- Texto secundário: #64748B

### Tipografia
- Família: Inter, system-ui, sans-serif
- Títulos: 600 (semibold)
- Corpo: 400 (regular)

---

## 6. Dados de Demonstração (Mock)

Para o protótipo, usar dados fictícios representativos:

### Setores
| Setor | Leitos | Ocupados | Disponíveis | Bloqueados |
|-------|--------|----------|-------------|------------|
| UTI Adulto | 10 | 9 | 1 | 0 |
| UTI Pediátrica | 6 | 4 | 2 | 0 |
| Enfermaria Clínica | 30 | 22 | 6 | 2 |
| Enfermaria Cirúrgica | 24 | 18 | 5 | 1 |
| Pediatria | 12 | 8 | 4 | 0 |
| Maternidade | 15 | 10 | 5 | 0 |
| **Total** | **97** | **71** | **23** | **3** |

### Indicadores
| Indicador | Valor | Meta | Status |
|-----------|-------|------|--------|
| Taxa de Ocupação | 73.2% | 80-85% | OK |
| TMP | 5.2 dias | 5 dias | Atenção |
| Rotatividade | 4.8 | 5.0 | OK |
| Previsão de altas (24h) | 8 | - | Info |

---

*Última atualização: 2026-03-28*
