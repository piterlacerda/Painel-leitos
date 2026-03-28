# Matriz de Indicadores de Gestão de Leitos

## Indicadores Essenciais

### 1. Taxa de Ocupação de Leitos
- **Definição:** Percentual de leitos ocupados em relação ao total disponível
- **Fórmula:** (Pacientes-dia / Leitos-dia disponíveis) × 100
- **Periodicidade:** Tempo real / Diário / Mensal
- **Meta referência:** 80-85% (ANAHp)
- **Uso:** Avaliar eficiência da utilização de recursos físicos
- **Fonte:** DATASUS, ANAHp, literatura

### 2. Tempo Médio de Permanência (TMP)
- **Definição:** Média de dias que os pacientes permanecem internados
- **Fórmula:** Total de pacientes-dia / Número de saídas (altas + óbitos + transferências)
- **Periodicidade:** Mensal
- **Meta referência:** Varia por especialidade (clínica: 5-7 dias; cirúrgica: 3-5 dias)
- **Uso:** Identificar gargalos, avaliar eficiência do fluxo
- **Fonte:** ANAHp, AHRQ

### 3. Índice de Rotatividade (Giro de Leitos)
- **Definição:** Número médio de pacientes que ocupam cada leito por período
- **Fórmula:** Número de saídas / Número de leitos operacionais
- **Periodicidade:** Mensal
- **Meta referência:** 4-6 pacientes/leito/mês
- **Uso:** Avaliar produtividade dos leitos
- **Fonte:** MS, ANAHp

### 4. Intervalo de Substituição
- **Definição:** Tempo médio que um leito permanece vago entre duas internações
- **Fórmula:** (Leitos-dia disponíveis - Pacientes-dia) / Número de saídas
- **Periodicidade:** Mensal
- **Meta referência:** < 1 dia
- **Uso:** Identificar ociosidade, melhorar fluxo de admissão
- **Fonte:** Literatura, ANAHp

### 5. Taxa de Readmissão em 30 dias
- **Definição:** Percentual de pacientes readmitidos em até 30 dias após alta
- **Fórmula:** (Readmissões em 30 dias / Total de altas) × 100
- **Periodicidade:** Mensal
- **Meta referência:** < 10% (geral); varia por condição clínica
- **Uso:** Indicador de qualidade assistencial e alta segura
- **Fonte:** CMS, AHRQ, ANS

---

## Indicadores Complementares

### 6. Taxa de Ocupação por Setor
- **Definição:** Ocupação estratificada por unidade (UTI, enfermaria, pediatria, etc.)
- **Uso:** Identificar setores com gargalos ou ociosidade

### 7. Previsão de Altas (próximas 24-48h)
- **Definição:** Número de pacientes com alta prevista pelo médico
- **Uso:** Planejamento de admissões, gestão de fluxo

### 8. Leitos Bloqueados
- **Definição:** Leitos indisponíveis por manutenção, limpeza ou falta de equipe
- **Fórmula:** (Leitos bloqueados / Leitos totais) × 100
- **Uso:** Identificar perdas de capacidade

### 9. Tempo de Espera para Internação (PS → Leito)
- **Definição:** Tempo desde a decisão de internar até a ocupação do leito
- **Meta referência:** < 4 horas
- **Uso:** Avaliar fluxo de admissão

### 10. Taxa de Mortalidade Hospitalar
- **Definição:** Óbitos / Total de saídas
- **Uso:** Indicador de qualidade assistencial (ajustar por case-mix)

---

## Fontes de Referência

| Fonte | Descrição |
|-------|-----------|
| ANAHp | Associação Nacional de Hospitais Privados - indicadores de desempenho |
| DATASUS | Dados públicos do SUS (SIH, CNES) |
| AHRQ | Agency for Healthcare Research and Quality (EUA) |
| CMS | Centers for Medicare & Medicaid Services (EUA) |
| ANS | Agência Nacional de Saúde Suplementar |
| ONA | Organização Nacional de Acreditação |
| JCI | Joint Commission International |

---

## Classificação por Dimensão

| Dimensão | Indicadores |
|----------|-------------|
| Eficiência | Taxa de ocupação, TMP, Rotatividade, Intervalo de substituição |
| Qualidade | Taxa de readmissão, Mortalidade |
| Acesso | Tempo de espera para internação |
| Operacional | Leitos bloqueados, Previsão de altas |

---

## Alertas Sugeridos no Painel

| Situação | Alerta | Cor |
|----------|--------|-----|
| Ocupação > 90% | Capacidade crítica | Vermelho |
| Ocupação < 60% | Ociosidade | Âmbar |
| Leito vago > 24h | Leito parado | Âmbar |
| TMP > meta do setor | Permanência elevada | Âmbar |
| Previsão de alta hoje | Oportunidade de admissão | Verde |

---

*Última atualização: 2026-03-28*
