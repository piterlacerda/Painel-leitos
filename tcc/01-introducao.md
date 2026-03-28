# 1. INTRODUÇÃO

## 1.1 Contextualização

A gestão de leitos hospitalares constitui um dos principais desafios enfrentados por instituições de saúde em todo o mundo. Os leitos representam recursos críticos e de alto custo, cuja utilização eficiente impacta diretamente a capacidade assistencial, os resultados financeiros e a qualidade do atendimento prestado à população (COSTA et al., 2020).

No contexto brasileiro, esse desafio assume proporções ainda maiores. O Sistema Único de Saúde (SUS), responsável pelo atendimento de aproximadamente 75% da população, enfrenta historicamente problemas de superlotação em emergências, filas de espera para internação e dificuldades na gestão do fluxo de pacientes (BRASIL, 2021). Paralelamente, o setor de saúde suplementar busca constantemente otimizar a utilização de seus recursos para garantir sustentabilidade financeira sem comprometer a qualidade assistencial (ANS, 2022).

A má gestão de leitos gera consequências em cadeia: pacientes aguardam por longos períodos em pronto-socorros, cirurgias eletivas são adiadas, há aumento do risco de infecções hospitalares, elevação dos custos operacionais e, em última instância, comprometimento dos desfechos clínicos (BITTENCOURT; HORTALE, 2009). Estudos demonstram que a superlotação hospitalar está associada ao aumento da mortalidade, maior tempo de permanência e redução da satisfação tanto de pacientes quanto de profissionais de saúde (MORLEY et al., 2018).

Nesse cenário, a tecnologia da informação emerge como aliada fundamental para a gestão hospitalar. Os Sistemas de Informação em Saúde (SIS) têm se consolidado como ferramentas essenciais para o monitoramento, a análise e a tomada de decisão em organizações de saúde (MARIN, 2010). Especificamente, os dashboards gerenciais — painéis visuais que apresentam indicadores-chave de desempenho em tempo real — têm demonstrado potencial significativo para aprimorar a gestão de recursos hospitalares (DOWDING et al., 2015).

A Organização Mundial da Saúde (OMS), por meio da Estratégia Global de Saúde Digital 2020-2025, enfatiza a importância da incorporação de tecnologias digitais para fortalecer os sistemas de saúde, melhorar a tomada de decisão e otimizar a alocação de recursos (WHO, 2021). No Brasil, políticas como a Estratégia de Saúde Digital para o Brasil 2020-2028 reforçam a necessidade de informatização e integração dos serviços de saúde (BRASIL, 2020).

Diante desse contexto, torna-se relevante investigar como sistemas digitais de monitoramento podem contribuir para a otimização da gestão de leitos hospitalares, integrando evidências científicas e boas práticas de gestão em uma proposta conceitual aplicável à realidade brasileira.

## 1.2 Problema de Pesquisa

A gestão de leitos hospitalares frequentemente carece de ferramentas que permitam monitoramento em tempo real e tomada de decisão baseada em dados. Muitas instituições ainda operam com controles manuais, planilhas descentralizadas ou sistemas de informação fragmentados, o que dificulta a visibilidade sobre a situação real dos leitos e compromete a capacidade de resposta dos gestores (SOUZA et al., 2019).

A ausência de indicadores padronizados e de mecanismos de alerta precoce contribui para a persistência de problemas como leitos ociosos em alguns setores enquanto outros enfrentam superlotação, demora na liberação de leitos após alta médica e dificuldade de previsão de demanda (BITTENCOURT; HORTALE, 2009).

Assim, emerge a seguinte questão de pesquisa:

**Como um sistema digital de monitoramento de indicadores pode contribuir para a otimização da gestão de leitos hospitalares?**

## 1.3 Justificativa

### 1.3.1 Relevância Institucional

Os leitos hospitalares representam um dos recursos mais onerosos das instituições de saúde. Estima-se que os custos associados à hotelaria hospitalar — que incluem a manutenção dos leitos — correspondam a uma parcela significativa do orçamento total das organizações (VECINA NETO; MALIK, 2016). A gestão ineficiente desses recursos resulta em desperdício financeiro e subutilização da capacidade instalada.

Por outro lado, hospitais que implementam sistemas de gestão de leitos baseados em indicadores reportam melhorias significativas em métricas como taxa de ocupação, tempo médio de permanência e rotatividade de leitos (KHANNA et al., 2017). Essas melhorias traduzem-se em maior capacidade de atendimento, redução de custos e melhores resultados assistenciais.

### 1.3.2 Relevância Científica

A literatura científica demonstra os benefícios de dashboards e sistemas de Business Intelligence (BI) na gestão hospitalar, porém poucos estudos brasileiros abordam especificamente a implementação prática de painéis de indicadores para gestão de leitos em hospitais de médio porte (REIS et al., 2017). Existe uma lacuna entre o conhecimento teórico disponível e a aplicação prática nas instituições de saúde do país.

Este trabalho contribui para a área de sistemas de informação em saúde ao propor uma arquitetura funcional de painel de indicadores baseada em evidências, com potencial de replicação em diferentes contextos institucionais.

### 1.3.3 Relevância Social

A otimização da gestão de leitos possui impacto direto na capacidade de atendimento à população. Leitos bem gerenciados significam mais pacientes atendidos, menor tempo de espera, redução de internações desnecessárias e melhor utilização dos recursos públicos e privados destinados à saúde (RAFFA; MALIK; PINOCHET, 2017).

No contexto do SUS, onde a demanda frequentemente supera a oferta, qualquer ganho de eficiência na gestão de leitos pode representar vidas salvas e sofrimento evitado. Assim, soluções tecnológicas que contribuam para essa eficiência possuem relevância social inegável.

### 1.3.4 Atualidade

A saúde digital é uma tendência consolidada globalmente. A pandemia de COVID-19 acelerou a adoção de tecnologias digitais nas instituições de saúde e evidenciou a importância do monitoramento em tempo real de recursos críticos como leitos de UTI (BRASIL, 2021). O momento é oportuno para propostas que integrem tecnologia e gestão em saúde.

No Brasil, iniciativas como o e-SUS e a Rede Nacional de Dados em Saúde (RNDS) criam um ambiente favorável para a implementação de sistemas de informação integrados, incluindo ferramentas de gestão de leitos (BRASIL, 2020).

## 1.4 Objetivos

### 1.4.1 Objetivo Geral

Desenvolver um protótipo conceitual de painel de indicadores para gestão de leitos hospitalares, fundamentado em evidências científicas e boas práticas de gestão em saúde.

### 1.4.2 Objetivos Específicos

1. Identificar, por meio de revisão de literatura, os principais indicadores utilizados na gestão de leitos hospitalares;

2. Analisar requisitos funcionais e técnicos para sistemas de monitoramento de leitos em instituições de saúde;

3. Propor a arquitetura funcional de um painel de indicadores para gestão de leitos;

4. Desenvolver um protótipo visual da solução proposta;

5. Discutir a viabilidade e potenciais benefícios da implementação em instituições de saúde brasileiras.

## 1.5 Referencial Teórico

### 1.5.1 Gestão de Leitos Hospitalares

A gestão de leitos hospitalares pode ser definida como o conjunto de processos e práticas destinados a otimizar a utilização dos leitos disponíveis, garantindo o equilíbrio entre demanda e oferta, a qualidade assistencial e a eficiência operacional (BITTENCOURT; HORTALE, 2009).

Os principais conceitos relacionados à gestão de leitos incluem:

**Taxa de Ocupação:** percentual de leitos ocupados em relação ao total disponível. É o indicador mais utilizado para avaliar a eficiência da utilização de leitos. A literatura recomenda taxas entre 80% e 85% como ideais, permitindo margem para flutuações de demanda sem superlotação (ANAHP, 2022).

**Tempo Médio de Permanência (TMP):** média de dias que os pacientes permanecem internados. Valores elevados podem indicar ineficiências no fluxo assistencial, complicações clínicas ou dificuldades na alta hospitalar (DIAS, 2015).

**Rotatividade de Leitos:** número médio de pacientes que ocupam cada leito em determinado período. Indica a produtividade dos leitos e está inversamente relacionada ao TMP (VECINA NETO; MALIK, 2016).

**Intervalo de Substituição:** tempo médio que um leito permanece vago entre duas internações consecutivas. Valores elevados sugerem problemas no fluxo de admissão ou na preparação dos leitos (ANAHP, 2022).

No contexto brasileiro, a gestão de leitos enfrenta desafios específicos, como a heterogeneidade dos serviços de saúde, a fragmentação dos sistemas de informação e as restrições orçamentárias, especialmente no setor público (SOUZA et al., 2019).

### 1.5.2 Sistemas de Informação em Saúde

Os Sistemas de Informação em Saúde (SIS) são definidos como conjuntos de elementos interligados que coletam, processam, armazenam e disseminam informações destinadas a apoiar a tomada de decisão, a gestão e a assistência em saúde (MARIN, 2010).

Os SIS podem ser classificados em diferentes níveis:

- **Nível Operacional:** sistemas de processamento de transações que registram atividades rotineiras (admissões, altas, transferências);
- **Nível Tático:** sistemas de informação gerencial que consolidam dados para apoiar o planejamento e controle;
- **Nível Estratégico:** sistemas de informação executiva que fornecem visão sintética para a alta gestão (DE SORDI, 2018).

Os benefícios dos SIS na gestão hospitalar incluem: melhoria na qualidade e segurança da assistência, apoio à tomada de decisão, integração de informações entre áreas e redução de retrabalho (PEREIRA et al., 2012).

Entretanto, a implementação de SIS enfrenta desafios como: fragmentação e baixa integração entre sistemas, custos elevados, resistência à mudança, problemas de qualidade dos dados e questões de segurança e privacidade (CINTHO; MACHADO; MORO, 2016).

### 1.5.3 Dashboards e Business Intelligence em Saúde

Dashboards são interfaces visuais que apresentam informações críticas de forma consolidada, permitindo o monitoramento de indicadores-chave de desempenho (Key Performance Indicators - KPIs) em uma única tela (FEW, 2006).

Na gestão hospitalar, dashboards têm sido utilizados para:

- Monitoramento de ocupação de leitos em tempo real;
- Acompanhamento de indicadores de qualidade e segurança;
- Visualização de tendências e padrões;
- Identificação precoce de problemas e oportunidades;
- Comunicação de resultados para diferentes níveis hierárquicos (DOWDING et al., 2015).

Estudos demonstram que a implementação de dashboards na gestão hospitalar está associada a melhorias em indicadores operacionais e clínicos. Khanna et al. (2017) reportaram redução de 8% no tempo médio de permanência após implementação de sistema de gestão de leitos com dashboard em hospital australiano.

Os princípios de design de dashboards efetivos incluem: simplicidade visual, hierarquia clara de informações, uso adequado de cores e alertas, atualização em tempo real e foco nas métricas mais relevantes para a tomada de decisão (FEW, 2006).

### 1.5.4 Tendências em Saúde Digital

A Organização Mundial da Saúde define saúde digital como o campo do conhecimento e prática associado ao uso de tecnologias digitais para melhorar a saúde (WHO, 2021). Isso inclui telemedicina, aplicativos móveis, inteligência artificial, Internet das Coisas (IoT) e sistemas de informação.

No Brasil, a Estratégia de Saúde Digital para o Brasil 2020-2028 estabelece diretrizes para a transformação digital do setor, incluindo:

- Informatização da Atenção Primária (e-SUS APS);
- Implantação da Rede Nacional de Dados em Saúde (RNDS);
- Adoção de padrões de interoperabilidade;
- Promoção da inovação em saúde digital (BRASIL, 2020).

Essas iniciativas criam um ambiente favorável para a implementação de sistemas de gestão de leitos integrados, que possam se comunicar com outros componentes do ecossistema de saúde digital brasileiro.

### 1.5.5 Indicadores de Desempenho em Gestão de Leitos

A seleção adequada de indicadores é fundamental para o sucesso de sistemas de monitoramento. Os indicadores devem ser relevantes, mensuráveis, acionáveis e baseados em dados disponíveis (DONABEDIAN, 1988).

Para a gestão de leitos, a literatura e entidades de referência como a Associação Nacional de Hospitais Privados (ANAHP) e a Organização Nacional de Acreditação (ONA) recomendam indicadores organizados em dimensões:

**Eficiência:** taxa de ocupação, tempo médio de permanência, rotatividade, intervalo de substituição.

**Qualidade:** taxa de readmissão em 30 dias, mortalidade hospitalar, eventos adversos relacionados à internação.

**Acesso:** tempo de espera para internação (do PS ao leito), tempo de espera em fila cirúrgica.

**Operacional:** leitos bloqueados, previsão de altas, tempo de liberação do leito após alta (ANAHP, 2022).

A combinação desses indicadores em um painel integrado permite visão abrangente da situação dos leitos e suporta a tomada de decisão em diferentes níveis gerenciais.

---

## Referências (parciais - seção Introdução)

ANAHP. Observatório 2022. São Paulo: Associação Nacional de Hospitais Privados, 2022.

ANS. Dados do Setor de Saúde Suplementar. Brasília: Agência Nacional de Saúde Suplementar, 2022.

BITTENCOURT, R. J.; HORTALE, V. A. Intervenções para solucionar a superlotação nos serviços de emergência hospitalar: uma revisão sistemática. Cadernos de Saúde Pública, v. 25, n. 7, p. 1439-1454, 2009.

BRASIL. Ministério da Saúde. Estratégia de Saúde Digital para o Brasil 2020-2028. Brasília: MS, 2020.

BRASIL. Ministério da Saúde. Painel de leitos e insumos COVID-19. Brasília: MS, 2021.

CINTHO, L. M. M.; MACHADO, R. R.; MORO, C. M. C. Métodos para avaliação de sistemas de informação em saúde. Journal of Health Informatics, v. 8, n. 2, 2016.

COSTA, A. L. et al. Gestão de leitos hospitalares: revisão integrativa. Revista de Enfermagem UFPE, v. 14, e243361, 2020.

DE SORDI, J. O. Administração da Informação. 3. ed. São Paulo: Saraiva, 2018.

DIAS, M. A. A. Gestão de leitos como ferramenta para melhoria da qualidade hospitalar. 2015. Dissertação (Mestrado) - FIOCRUZ, Rio de Janeiro, 2015.

DONABEDIAN, A. The quality of care: how can it be assessed? JAMA, v. 260, n. 12, p. 1743-1748, 1988.

DOWDING, D. et al. Dashboards for improving patient care: review of the literature. International Journal of Medical Informatics, v. 84, n. 2, p. 87-100, 2015.

FEW, S. Information Dashboard Design: The Effective Visual Communication of Data. Sebastopol: O'Reilly Media, 2006.

KHANNA, S. et al. Impact of admission prediction for improved hospital bed management. Annals of Operations Research, v. 263, n. 1-2, p. 91-104, 2017.

MARIN, H. F. Sistemas de informação em saúde: considerações gerais. Journal of Health Informatics, v. 2, n. 1, p. 20-24, 2010.

MORLEY, C. et al. Emergency department crowding: A systematic review of causes, consequences and solutions. PLOS ONE, v. 13, n. 8, e0203316, 2018.

PEREIRA, S. R. et al. Sistemas de informação para gestão hospitalar. Journal of Health Informatics, v. 4, n. 4, p. 170-175, 2012.

RAFFA, C.; MALIK, A. M.; PINOCHET, L. H. C. Uso de tecnologia da informação em hospitais de São Paulo. Revista de Administração de Empresas, v. 57, n. 2, p. 161-175, 2017.

REIS, Z. S. N. et al. Análise de dados em saúde: desafios e perspectivas. Journal of Health Informatics, v. 9, n. 3, 2017.

SOUZA, A. A. et al. Gestão de leitos em hospital público de Minas Gerais. Revista de Administração Hospitalar e Inovação em Saúde, v. 16, n. 3, p. 30-45, 2019.

VECINA NETO, G.; MALIK, A. M. Gestão em Saúde. 2. ed. Rio de Janeiro: Guanabara Koogan, 2016.

WHO. Global Strategy on Digital Health 2020-2025. Geneva: World Health Organization, 2021.
