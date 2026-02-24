![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)

<div align="center">
  
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![IFRS 9](https://img.shields.io/badge/IFRS%209-Compliance-blue?style=for-the-badge)
![Basileia III](https://img.shields.io/badge/Basileia%20III-Capital%20Regulatório-orange?style=for-the-badge)

</div>

<div align="center">

# 📊 Credit Risk Dashboard

### Plataforma executiva para gestão estratégica de risco de crédito e capital regulatório

Simulação de cenários, monitoramento IFRS 9, análise de concentração, inadimplência e capital regulatório —  
com profundidade técnica e orientação direta à tomada de decisão.

</div>

---

## 🧠 Sobre o Projeto

Solução analítica **end-to-end** para gestão institucional de risco de crédito.

O projeto reúne:

- +170 métricas financeiras e regulatórias  
- 137 medidas DAX organizadas por domínio  
- Conformidade com IFRS 9 (Stage 1, 2 e 3 + ECL 12M e Lifetime)  
- Simulador de Stress Test com recálculo em tempo real  
- Parâmetros dinâmicos de métricas e período  
- Glossário técnico integrado ao modelo  

Desenvolvido com a linguagem, estrutura e profundidade conceitual do mercado financeiro.

---

## 📋 Sumário

- [🎯 Visão Geral](#visao-geral)
- [💡 Problema & Solução](#problema-solucao)
- [🏗️ Arquitetura do Modelo](#arquitetura-do-modelo)
- [📦 Módulos Analíticos](#modulos-analiticos)
- [📈 Métricas-Chave e Conceitos do Setor](#metricas-chave)
- [🎛️ Diferenciais Técnicos e de UX](#diferenciais-tecnicos)
- [🧪 Stress Test Interativo](#stress-test)
- [📖 Glossário de Termos](#glossario)
- [🎯 Impacto no Negócio](#impacto-negocio)
- [🛠️ Tecnologias Utilizadas](#tecnologias)
- [🔧 Como Utilizar](#como-utilizar)
- [📧 Contato](#contato)

---

<a id="visao-geral"></a>

# 🎯 Visão Geral

Este projeto entrega uma **solução completa para monitoramento de risco de crédito**, construída integralmente em Power BI, com modelagem Star Schema e engine DAX robusta.

O dashboard cobre:

- Portfólio e concessão
- Inadimplência e NPL
- IFRS 9 (Stage 1, 2 e 3)
- ECL 12M e Lifetime
- Concentração (HHI)
- Vintage & MOB
- Early Warning System
- Stress Testing com parâmetro dinâmico

Mais do que um relatório, trata-se de uma **plataforma analítica executiva orientada à decisão**.

---

# 📊 Números do Projeto

| Componente | Volume |
|------------|--------|
| Medidas DAX | **137 medidas organizadas** |
| Indicadores funcionais | **+170 métricas** |
| Tabelas no modelo | **18 tabelas** |
| Relacionamentos | **12 relacionamentos ativos** |
| Glossário interno | **127 definições documentadas** |
| Módulos analíticos | **6 módulos independentes** |

---

<a id="problema-solucao"></a>

# 💡 Problema & Solução

| 🔴 Desafio de Mercado | ✅ Implementação no Projeto |
|----------------------|----------------------------|
| Relatórios estáticos | Parâmetros dinâmicos de período e métricas |
| Falta de visão IFRS 9 estruturada | Staging automático + ECL 12M & Lifetime |
| Incapacidade de simular cenários | Stress Test com recálculo integral em tempo real |
| Falta de padronização conceitual | Glossário técnico integrado ao modelo |
| Análises fragmentadas | Estrutura modular unificada |

---

<a id="arquitetura-do-modelo"></a>

# 🏗️ Arquitetura do Modelo

## 📐 Star Schema

- 3 tabelas fato (Carteira, Risco, Provisão)
- Dimensões compartilhadas (Cliente, Produto, Tempo, Rating)
- Tabelas auxiliares para parâmetros dinâmicos
- Tabela organizadora de medidas

**Decisão arquitetural:** separação por domínio de negócio para preservar granularidade e performance DAX.

---

<a id="modulos-analiticos"></a>

# 📦 Módulos Analíticos

## 1️⃣ Portfólio

- Saldo Carteira
- Total Concedido
- Ticket Médio
- Spread
- Prazo Médio
- % Garantida
- Crescimento MoM / YoY

---

## 2️⃣ Risco & Inadimplência

- Over 30 / 60 / 90
- Ativo Problemático
- NPL R$ e NPL Ratio
- Roll Rates
- PD Média
- LGD
- EAD 1 / 2 / 3
- ECL 12M e Lifetime

---

## 3️⃣ Concentração

- HHI
- Top 10 Clientes
- Concentração por Produto
- Concentração por Segmento
- Concentração Geográfica

---

## 4️⃣ Performance

- Recuperação R$
- Taxa de Write-Off
- Coverage NPL
- Eficiência de Provisão
- ROE
- Capital Basel

---

## 5️⃣ Análise Avançada

- Vintage por Safra
- MOB
- Early Warning System (0–100)
- Score de Deterioração
- Correlação PD × LGD

---

## 6️⃣ Stress Test & Cenários

Simulação interativa de choque na PD com impacto automático em:

- ECL
- NPL Ratio
- Coverage
- Provisão Necessária
- Capital Regulatório

---

<a id="metricas-chave"></a>

## 📈 Métricas-Chave e Conceitos do Setor

> Esta seção apresenta os indicadores centrais de risco de crédito implementados no modelo — com conceito de mercado, relevância regulatória, aplicação prática e implementação DAX. O objetivo é demonstrar que o projeto vai além da técnica: reflete entendimento real do negócio bancário e financeiro.

---

### 📌 EAD — Exposure at Default

**O que é:** O EAD representa o valor total da exposição de uma instituição financeira no momento em que uma contraparte entra em default. É a estimativa do saldo que ficaria em aberto caso o cliente não honrasse suas obrigações na data do evento de crédito.

**Por que importa:** É a base quantitativa do modelo de perda esperada. Junto com PD e LGD, forma o tripé do cálculo do ECL conforme IFRS 9 e do capital regulatório conforme Basileia III: `Perda Esperada = PD × LGD × EAD`. A segmentação do EAD por stage IFRS 9 permite monitorar em tempo real a migração de risco na carteira — um crescimento do EAD 3 sobre o total indica deterioração estrutural.

**No modelo:** O EAD é segmentado nos três estágios do IFRS 9 e acompanhado em valor absoluto e percentual, com séries históricas para análise evolutiva.

```dax
-- EAD Total da carteira
EAD = SUM(FATO_RISCO[ead])

-- EAD Stage 1: operações sem aumento significativo de risco
EAD 1 =
CALCULATE(
    SUM(FATO_RISCO[ead]),
    FATO_RISCO[stage_ifrs9] = 1
)

-- EAD Stage 3: operações com evidência de imparidade (default incorrido)
EAD 3 =
CALCULATE(
    SUM(FATO_RISCO[ead]),
    FATO_RISCO[stage_ifrs9] = 3
)

-- Percentual do EAD em Stage 3 — indicador de concentração de risco
% EAD 3 = DIVIDE([EAD 3], [EAD])
```

---

### 📌 PD — Probability of Default

**O que é:** A PD é a probabilidade estimada de que um devedor entre em default dentro de um horizonte temporal definido. Para operações em Stage 1, o horizonte é de 12 meses. Para Stage 2 e 3, a PD é calculada para a vida remanescente do contrato (Lifetime PD).

**Por que importa:** A PD é o principal input dos modelos de rating, precificação de crédito e cálculo de ECL. Uma `PD Média` crescente na carteira sinaliza piora da qualidade creditícia e exige revisão das políticas de concessão. A diferença entre `PD Inicial` (na originação) e `PD Média` atual revela o quanto a carteira se deteriorou desde a concessão — um delta elevado é sinal de alerta para o time de risco.

**No modelo:** Monitoradas separadamente por stage, com série histórica e uso no simulador de stress test.

```dax
-- PD Média atual, ponderada pelo EAD (padrão de mercado)
PD Média =
DIVIDE(
    SUMX(FATO_RISCO, FATO_RISCO[pd] * FATO_RISCO[ead]),
    SUM(FATO_RISCO[ead])
)

-- PD Inicial: baseline de risco na originação
PD Inicial =
DIVIDE(
    SUMX(FATO_RISCO, FATO_RISCO[pd_inicial] * FATO_RISCO[ead]),
    SUM(FATO_RISCO[ead])
)

-- PD Stage 2: risco elevado, abaixo do default
PD Stage 2 =
CALCULATE([PD Média], FATO_RISCO[stage_ifrs9] = 2)
```

---

### 📌 LGD — Loss Given Default

**O que é:** O LGD representa a proporção da exposição que de fato será perdida em caso de default, após todos os processos de recuperação, execução de garantias e colaterais. É expresso como percentual do EAD e varia de 0% (recuperação total) a 100% (perda integral).

**Por que importa:** O LGD reflete a qualidade das garantias da carteira e a eficiência do processo de recuperação. Operações com garantia real (imóveis, veículos) tendem a LGD de 20–40%, enquanto crédito pessoal não garantido pode atingir 80–90%. No modelo, a correlação entre PD e LGD (`Corr PD-LGD`) é monitorada: quando ambas crescem simultaneamente, há sinal de estresse sistêmico na carteira.

```dax
-- LGD Médio ponderado pelo EAD
LGD =
DIVIDE(
    SUMX(FATO_RISCO, FATO_RISCO[lgd] * FATO_RISCO[ead]),
    SUM(FATO_RISCO[ead])
)

-- Correlação PD × LGD: indicador de estresse sistêmico
Corr PD-LGD =
VAR MediaPD = [PD Média]
VAR MediaLGD = [LGD]
RETURN
    DIVIDE(
        SUMX(FATO_RISCO,
            (FATO_RISCO[pd] - MediaPD) * (FATO_RISCO[lgd] - MediaLGD)),
        COUNTROWS(FATO_RISCO)
    )
```

---

### 📌 ECL — Expected Credit Loss (IFRS 9)

**O que é:** O ECL é a perda de crédito esperada calculada conforme a norma **IFRS 9**, adotada no Brasil via Resolução CMN 4.966/2021. Diferencia-se do modelo anterior de perda incorrida por ser **prospectivo**: incorpora cenários macroeconômicos futuros e não apenas perdas já observadas.

**Por que importa:** O IFRS 9 exige que as instituições constituam provisão com base no ECL em dois horizontes: **ECL 12 meses** para operações Stage 1 (sem deterioração de risco) e **ECL Lifetime** para Stage 2 e 3 (risco significativamente elevado ou em default). O gap entre ECL calculado e provisão contabilmente constituída (`Gap Provisão`) é crítico para a gestão de capital e para a antecipação de impactos no resultado.

```dax
-- ECL Total: 12M para Stage 1, Lifetime para Stage 2 e 3
ECL =
SUMX(
    FATO_RISCO,
    IF(FATO_RISCO[stage_ifrs9] = 1,
        FATO_RISCO[ecl_12m],
        FATO_RISCO[ecl_lifetime]
    )
)

-- Expected Loss pelo modelo interno (PD × LGD × EAD)
Expected Loss =
SUMX(FATO_RISCO,
    FATO_RISCO[pd] * FATO_RISCO[lgd] * FATO_RISCO[ead]
)

-- Gap entre ECL e provisão constituída: risco de underprovisioning
Gap Provisão = [ECL] - [Provisão]

-- Eficiência da provisão: quanto do ECL está coberto
Efic Provisão = DIVIDE([Provisão], [ECL])
```

---

### 📌 Over — Faixas de Atraso

**O que é:** As faixas de atraso classificam as operações pelo número de dias em que estão sem pagamento. As faixas padrão de mercado são: **Over 30** (1–30 dias), **Over 60** (31–60 dias), **Over 90** (61–90 dias) e **Ativo Problemático** (acima de 90 dias). Cada faixa corresponde, em termos gerais, a um estágio de deterioração da qualidade de crédito.

**Por que importa:** As faixas são os indicadores operacionais mais imediatos de deterioração. Permitem dimensionar o provisionamento, acionar as equipes de cobrança preventiva e antecipar a migração para o NPL. O crescimento acelerado do Over 30 é o primeiro sinal de entrada no ciclo de inadimplência — detectado antes que o risco se materialize nos indicadores mais tardios.

```dax
-- Over 30: operações com 1 a 30 dias de atraso
Over 30 =
CALCULATE(SUM(FATO_RISCO[ead]),
    FATO_RISCO[dias_atraso] >= 1 &&
    FATO_RISCO[dias_atraso] <= 30)

-- Over 60: 31 a 60 dias
Over 60 =
CALCULATE(SUM(FATO_RISCO[ead]),
    FATO_RISCO[dias_atraso] >= 31 &&
    FATO_RISCO[dias_atraso] <= 60)

-- Over 90: 61 a 90 dias (limiar crítico antes do NPL)
Over 90 =
CALCULATE(SUM(FATO_RISCO[ead]),
    FATO_RISCO[dias_atraso] >= 61 &&
    FATO_RISCO[dias_atraso] <= 90)

-- Ativo Problemático: >90 dias (equivalente ao Stage 3 IFRS 9)
Ativo Problemático =
CALCULATE(SUM(FATO_RISCO[ead]),
    FATO_RISCO[dias_atraso] > 90)

-- Percentual sobre o saldo total da carteira
% Over 30 = DIVIDE([Over 30], [Saldo Carteira])
```

---

### 📌 NPL — Non-Performing Loans

**O que é:** O NPL (Non-Performing Loans) engloba as operações com mais de 90 dias de atraso, classificadas como crédito problemático pelo mercado. O **NPL Ratio** — razão entre o saldo NPL e o saldo total da carteira — é o indicador de inadimplência mais monitorado por analistas, reguladores e investidores.

**Por que importa:** O NPL Ratio é um KPI primário de qualidade de portfólio em qualquer instituição financeira. Um NPL crescente pressiona as linhas de provisão, reduz o lucro líquido ajustado ao risco (RAROC) e pode sinalizar deterioração estrutural do modelo de crédito. Reguladores como o Bacen monitoram o NPL como indicador de solidez do sistema financeiro. No modelo, o NPL é acompanhado com série histórica, índice de evolução e integração com os estágios IFRS 9.

```dax
-- NPL R$: saldo das operações com mais de 90 dias de atraso
NPL R$ =
CALCULATE(SUM(FATO_RISCO[ead]),
    FATO_RISCO[dias_atraso] > 90)

-- NPL Ratio: principal indicador de inadimplência
NPL Ratio = DIVIDE([NPL R$], [Saldo Carteira])

-- NPL Evolution Index: variação normalizada do NPL (base 100)
NPL Evolution Index =
DIVIDE(
    [NPL Ratio],
    CALCULATE([NPL Ratio],
        FIRSTDATE(DIM_TEMPO[data_base]))
) * 100
```

---

### 📌 WO — Write-Off

**O que é:** O write-off é o processo contábil de baixa definitiva de operações classificadas como irrecuperáveis — tipicamente acima de 180 ou 360 dias de atraso, conforme a política de crédito da instituição. Após a baixa, a operação sai do balanço ativo; os esforços de recuperação extrajudicial e judicial, contudo, continuam.

**Por que importa:** A `Taxa WO` mede o fluxo de baixas como percentual da carteira total — indicador de maturidade do ciclo de inadimplência. A relação entre write-off e recuperação (`Recup vs WO`) revela a eficiência real do processo de cobrança pós-baixa e o retorno líquido sobre o portfólio problemático.

```dax
-- WO R$: saldo elegível para write-off (>180 dias)
WO R$ =
CALCULATE(SUM(FATO_RISCO[ead]),
    FATO_RISCO[dias_atraso] > 180)

-- Taxa de Write-off sobre a carteira total
Taxa WO = DIVIDE([WO R$], [Saldo Carteira])

-- Comparativo recuperação × write-off
Recup vs WO =
DIVIDE([Recup R$], [Recup R$] + [WO R$])
```

---

### 📌 Roll Rates — Taxas de Migração entre Faixas

**O que é:** As Roll Rates medem a proporção de operações (ou saldo) que migra de uma faixa de atraso para a seguinte em um dado período. São calculadas para cada transição possível: Adimplente → 1-30, 1-30 → 31-60, 31-60 → 61-90 e 61-90 → 91+.

**Por que importa:** São amplamente utilizadas em modelos preditivos de crédito e no dimensionamento de provisões dinâmicas. Uma Roll Rate crescente no início do funil (Adim → 1-30) indica aumento do fluxo de entrada em inadimplência — sinal de alerta para a política de concessão. Roll Rates elevadas nas faixas tardias sinalizam ineficiência da cobrança intermediária e antecipam pressão sobre o NPL nos meses seguintes.

```dax
-- Roll Rate: Adimplente → 1-30 dias (taxa de entrada em atraso)
RR Adim→1-30 =
DIVIDE(
    CALCULATE([Over 30], DATEADD(DIM_TEMPO[data_base], 0, MONTH)),
    CALCULATE([Qtd Adimplentes], DATEADD(DIM_TEMPO[data_base], -1, MONTH))
)

-- Roll Rate: 1-30 → 31-60 dias (efetividade da cobrança inicial)
RR 1-30→31-60 =
DIVIDE(
    CALCULATE([Over 60], DATEADD(DIM_TEMPO[data_base], 0, MONTH)),
    CALCULATE([Over 30], DATEADD(DIM_TEMPO[data_base], -1, MONTH))
)
```

---

### 📌 HHI — Índice Herfindahl-Hirschman

**O que é:** O HHI é um índice econômico de concentração que mede a distribuição do saldo da carteira entre os tomadores. Calculado como a soma dos quadrados da participação percentual de cada cliente, varia de 0 (carteira perfeitamente dispersa) a 10.000 (concentração total em um único tomador).

**Por que importa:** Reguladores e gestores de risco utilizam o HHI para identificar risco de concentração — um risco sistêmico que pode comprometer toda a carteira caso poucos tomadores entrem em default simultaneamente. A classificação (`HHI Class`) segue os parâmetros internacionais: abaixo de 1.500 (baixa concentração), 1.500–2.500 (concentração moderada), acima de 2.500 (alta concentração).

---

### 📌 MOB — Months on Books e Análise de Vintage

**O que é:** MOB é o número de meses decorridos desde a data de concessão de cada operação. A análise de **Vintage** agrupa operações pelo período de originação (safra) e monitora a evolução da inadimplência ao longo do MOB — permitindo comparar o desempenho de diferentes coortes de crédito.

**Por que importa:** É o instrumento mais poderoso para avaliação da qualidade dos critérios de concessão ao longo do tempo. Uma safra com NPL Ratio alto aos 12 MOB indica que o modelo de crédito daquele período estava mal calibrado — informação fundamental para a revisão de políticas de aprovação. Bancos e financeiras utilizam curvas de vintage como insumo central dos modelos de PD e provisionamento prospectivo.

---

<a id="diferenciais-tecnicos"></a>

## 🎛️ Diferenciais Técnicos e de UX

### 📊 Parâmetro de Métricas — Tabela Analítica com Colunas Configuráveis

Um dos maiores diferenciais do projeto é a implementação de uma **tabela analítica com colunas totalmente configuráveis pelo usuário**. Por meio da tabela `d_metrica`, o analista seleciona quais indicadores deseja exibir — e a tabela se reconstrói automaticamente, apresentando Valor Atual, Valor Anterior, Variação Absoluta e Variação Percentual para cada métrica selecionada, segmentada por qualquer dimensão disponível.

```
Painel de Seleção (usuário escolhe quais métricas exibir):
┌─────────────────┬───────────────────────────────┐
│ ● Saldo Carteira│ ○ LGD                         │
│ ● EAD           │ ○ PD Inicial                  │
│ ● EAD 1         │ ○ PD Média                    │
│ ○ EAD 2         │ ○ Cobertura ECL               │
│ ○ EAD 3         │ ● NPL Ratio                   │
│ ○ % EAD 1       │ ● Taxa Inadimplência          │
└─────────────────┴───────────────────────────────┘

Resultado na tabela analítica (gerado dinamicamente):
┌──────────────┬─────────────────────────┬─────────────────────────┬────...
│              │          EAD            │          EAD 1          │
│ Tipo Cliente │ Atual · Anterior · Var% │ Atual · Anterior · Var% │
├──────────────┼─────────────────────────┼─────────────────────────┼────...
│ PF           │ 39,3Mi · 43,4Mi · -9,4% │ 36,3Mi · 39,7Mi · -8,4%│
│ PJ           │ 16,4Mi · 17,4Mi · -5,8% │ 14,8Mi · 15,1Mi · -2,0%│
│ Total        │ 55,7Mi · 60,8Mi · -8,4% │ 51,0Mi · 54,8Mi · -6,9%│
└──────────────┴─────────────────────────┴─────────────────────────┴────...
```

Qualquer combinação de métrica, dimensão e período é configurável pelo usuário final — sem necessidade de editar o relatório ou criar novas páginas.

```dax
-- Resolução dinâmica: cada ID da d_metrica mapeia para uma medida real
Métrica Selecionada =
VAR IDSel = SELECTEDVALUE(d_metrica[id])
RETURN
    SWITCH(IDSel,
        0,  [Saldo Carteira],
        1,  [EAD],
        2,  [EAD 1],
        3,  [EAD 2],
        4,  [EAD 3],
        8,  [Over 30],
        16, [NPL Ratio],
        17, [NPL R$],
        19, [Taxa Inadimplência],
        21, [PD Média],
        -- + 45 outras métricas mapeadas
        BLANK()
    )

-- Título dinâmico gerado automaticamente a partir da seleção
Nome Métrica = SELECTEDVALUE(d_metrica[d_metrica], "Selecione uma Métrica")

-- Variação absoluta entre período atual e anterior
Variação Absoluta = [Valor Atual] - [Valor Anterior]

-- Variação percentual
Variação % = DIVIDE([Variação Absoluta], [Valor Anterior])
```

---

### 📅 Parâmetro de Período — Comparativo Temporal Dinâmico

O modelo implementa um **seletor de período de comparação** (`d_periodo`) que permite ao analista escolher qualquer mês histórico como referência. Todas as variações do modelo são recalculadas automaticamente — eliminando a rigidez do "mês anterior fixo" que limita a maioria dos dashboards tradicionais.

```
Exemplos de uso:
┌──────────────────────┬──────────────────────┬────────────────────────┐
│    282,47 Mil        │    745,76 Mil         │  Comparar com: [ 3 ] ▼ │
│    DEZ/25            │    SET/25             │  (seleção do usuário)  │
└──────────────────────┴──────────────────────┴────────────────────────┘

Parâmetro "3" → compara DEZ/25 vs. SET/25  (janela trimestral)
Parâmetro "1" → compara DEZ/25 vs. NOV/25  (variação mensal — MoM)
Parâmetro "12" → compara DEZ/25 vs. DEZ/24 (variação anual — YoY)
Parâmetro "6" → compara DEZ/25 vs. JUN/25  (janela semestral)
```

Esse recurso transforma o dashboard em uma ferramenta de análise comparativa estratégica, não apenas um relatório de posição.

```dax
-- Período de comparação selecionado via parâmetro
Mês Anterior =
CALCULATE(
    [Métrica Selecionada],
    DATEADD(DIM_TEMPO[data_base], -[Valor d_periodo], MONTH)
)

-- Variação percentual em relação ao período selecionado
Variação % =
DIVIDE([Valor Atual] - [Mês Anterior], [Mês Anterior])
```

---

### 📉 Bookmarks — Agrupamento Dinâmico de Gráficos

Gráficos com múltiplas perspectivas analíticas são controlados por **botões de navegação com bookmarks**, permitindo ao usuário alternar entre agrupamentos distintos sem sair da página. O gráfico de Distribuição Evolutiva, por exemplo, oferece quatro visões acionadas por botão:

```
[ EADs ]  [ % EADs ]  [ Over e Ap ]  [ % Over e Ap ]
    ↑
  Usuário clica → dados, séries, escala e título
  mudam instantaneamente via estado de bookmark
```

Cada botão aciona um estado pré-configurado que altera os dados exibidos, as séries do gráfico, a escala do eixo e o título — de forma coordenada e instantânea. Essa abordagem mantém o dashboard coeso e a experiência fluida, sem proliferação de páginas para análises correlatas sobre o mesmo tema.

---

### ✨ Storytelling com Ícones Animados

O dashboard incorpora **ícones animados** de forma estratégica nos cards de KPI e nos alertas do Early Warning System. A animação é aplicada com critério editorial: reforça visualmente sinais de alerta (NPL crescente, EWS em nível Alto ou Crítico, Coverage abaixo do threshold regulatório) sem comprometer a densidade informacional da página — seguindo boas práticas de **data storytelling** para ambientes executivos.

---

<a id="stress-test"></a>

## 🧪 Stress Test Interativo

O módulo de Stress Test implementa um **simulador de cenários adversos com entrada paramétrica**, permitindo ao analista aplicar choques na Probability of Default (PD) da carteira e visualizar instantaneamente o impacto cascata em todas as métricas de risco, provisão e capital — sem reconstruir o modelo ou criar relatórios paralelos.

### Como funciona o simulador

```
┌─────────────────────────────────────────────────────────────────────┐
│                                                                     │
│  ENTRADA                                                            │
│  Usuário seleciona o multiplicador de stress via parâmetro          │
│  Exemplo: Stress PD % = 4 → PD será 4× a PD atual da carteira      │
│                                                                     │
│  p_stress_test captura o valor → [% Stress] resolve a entrada       │
│                                                                     │
│  Stress PD Média = PD Média × (1 + % Stress)                        │
│                                                                     │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  PROPAGAÇÃO — todos os outputs são recalculados em tempo real       │
│                                                                     │
│  Stress ECL          → ECL total com a nova PD estressada           │
│  Stress ECL %        → Variação percentual vs. cenário base         │
│  Stress NPL Ratio    → NPL Ratio projetado no cenário adverso       │
│  % Stress EAD 3      → Migração projetada de EAD para Stage 3       │
│  Stress Coverage     → Coverage Ratio no cenário estressado         │
│  Stress Provisão     → Provisão adicional que seria necessária      │
│  Stress Provisão Nec → Provisão total necessária no cenário stress  │
│  Stress Capital      → Capital regulatório adicional requerido      │
│                                                                     │
├─────────────────────────────────────────────────────────────────────┤
```

### Por que isso importa

Em instituições financeiras, testes de estresse são obrigatórios para gestão de capital (Basileia III) e para avaliação da capacidade da carteira de absorver choques macroeconômicos. O simulador deste projeto traduz esse processo regulatório em uma ferramenta interativa e acessível, permitindo que analistas e gestores tomem decisões de provisão e capital com base em cenários prospectivos — não apenas na posição histórica.

```dax
-- PD estressada dinamicamente via parâmetro
Stress PD Média =
VAR PctStress = [% Stress]
RETURN [PD Média] * (1 + PctStress)

-- ECL recalculado com a PD estressada (cap em 100%)
Stress ECL =
SUMX(
    FATO_RISCO,
    MIN([Stress PD Média], 1) * FATO_RISCO[lgd] * FATO_RISCO[ead]
)

-- Impacto percentual incremental vs. ECL do cenário base
Stress ECL % = DIVIDE([Stress ECL] - [ECL], [ECL])

-- Provisão adicional necessária para cobrir o ECL estressado
Stress Provisão = [Stress ECL] - [Provisão]

-- Capital regulatório adicional no cenário de stress
Stress Capital = [Stress ECL] * 0.11 -- alíquota Basileia III
```

---

<a id="glossario"></a>

## 📖 Glossário de Termos

> Glossário dos principais termos técnicos e regulatórios utilizados no projeto — do mercado financeiro à implementação em Power BI.

---

### Termos de Risco de Crédito

| Termo | Definição |
|---|---|
| **PD** (Probability of Default) | Probabilidade estimada de que um devedor entre em default dentro de um horizonte temporal. Base de todos os modelos de precificação de risco e cálculo de ECL. |
| **LGD** (Loss Given Default) | Percentual da exposição que se perde efetivamente em caso de default, após recuperação e execução de garantias. Varia de 0% a 100%. |
| **EAD** (Exposure at Default) | Valor total da exposição financeira no momento do default. Junto com PD e LGD, compõe o tripé do cálculo de perda esperada. |
| **ECL** (Expected Credit Loss) | Perda de crédito esperada conforme IFRS 9. Calculada de forma prospectiva, incorporando cenários macroeconômicos futuros — diferente do modelo anterior de perda incorrida. |
| **ECL 12M** | ECL calculado para um horizonte de 12 meses. Aplicado às operações Stage 1 (sem deterioração significativa de risco). |
| **ECL Lifetime** | ECL calculado para toda a vida remanescente do contrato. Aplicado às operações Stage 2 e 3 (risco elevado ou em default). |
| **Expected Loss** | Perda esperada pelo modelo interno: `PD × LGD × EAD`. Métrica complementar ao ECL IFRS 9. |
| **NPL** (Non-Performing Loans) | Carteira de crédito com operações em atraso superior a 90 dias. O NPL Ratio (NPL / Carteira Total) é o principal KPI de inadimplência do mercado. |
| **Over 30 / 60 / 90** | Faixas de classificação de operações pelo número de dias em atraso: 1–30, 31–60 e 61–90 dias, respectivamente. |
| **Ativo Problemático** | Operações com mais de 90 dias de atraso. Equivalente conceitual ao Stage 3 do IFRS 9. |
| **Roll Rate** | Taxa de migração de operações de uma faixa de atraso para a seguinte. Usada em modelos preditivos e calibração de provisões dinâmicas. |
| **Write-Off (WO)** | Baixa contábil de operações irrecuperáveis (tipicamente >180 dias). A operação sai do balanço ativo, mas os esforços de recuperação continuam. |
| **Coverage Ratio** | Taxa de cobertura da provisão sobre a carteira inadimplente. `Coverage NPL = Provisão / NPL R$`. Quanto maior, mais protegida está a instituição. |
| **Spread** | Diferença entre a taxa cobrada ao cliente e o custo de captação da instituição. Proxy de rentabilidade ajustada ao risco. |
| **LTV** (Loan-to-Value) | Razão entre o saldo devedor e o valor da garantia. LTV alto indica menor proteção em caso de execução da garantia. |

---

### Termos de IFRS 9 e Regulação

| Termo | Definição |
|---|---|
| **IFRS 9** | Norma contábil internacional de instrumentos financeiros (vigente no Brasil via CMN 4.966/2021). Substituiu o IAS 39 com a adoção do modelo de perda esperada (vs. perda incorrida). |
| **Stage 1** | Operações sem aumento significativo de risco de crédito desde a originação. Provisão: ECL 12 meses. |
| **Stage 2** | Operações com aumento significativo de risco desde a originação (mas sem default). Provisão: ECL Lifetime. |
| **Stage 3** | Operações com evidência objetiva de imparidade (default incorrido). Provisão: ECL Lifetime com PD ≈ 100%. |
| **Migration Rate** | Taxa de migração entre stages IFRS 9 em um período. `Migration 1→2` e `Migration 2→3` são indicadores de deterioração progressiva. |
| **Aumento Significativo de Risco** | Critério do IFRS 9 para migração ao Stage 2. Pode ser baseado em dias de atraso (>30 dias), variação da PD, renegociações ou fatores qualitativos. |
| **Basileia III** | Acordo internacional de regulação bancária (BIS). Define os requerimentos mínimos de capital, liquidez e alavancagem para instituições financeiras. |
| **Capital Regulatório** | Capital mínimo exigido pelo regulador para absorver perdas inesperadas. No modelo, calculado como 11% do EAD ponderado pelo risco (RWA simplificado). |
| **Stress Test** | Simulação de cenários adversos para avaliar a resiliência do portfólio. Reguladores como o Bacen e o BCE realizam stress tests periódicos no sistema bancário. |

---

### Termos de Análise Avançada

| Termo | Definição |
|---|---|
| **Vintage** | Coorte de operações agrupadas pela data de originação (safra). A análise de vintage compara a evolução da inadimplência de diferentes safras ao longo do MOB. |
| **MOB** (Months on Books) | Número de meses decorridos desde a data de concessão de cada operação. Eixo temporal da análise de vintage. |
| **HHI** (Índice Herfindahl-Hirschman) | Índice de concentração de mercado. Em crédito, mede a dispersão do saldo entre tomadores. Abaixo de 1.500 = baixa concentração; acima de 2.500 = alta concentração. |
| **EWS** (Early Warning System) | Sistema de alertas antecipados que monitora indicadores-líderes de deterioração (atraso leve, migração Stage 1→2, variação de PD) antes que o risco se materialize no NPL. |
| **IQC** (Índice de Qualidade da Carteira) | Índice composto 0–100 que sintetiza múltiplos indicadores de qualidade em uma única métrica. Quanto mais próximo de 100, melhor a qualidade da carteira. |
| **Score Risco** | Score composto 0–100 que combina inadimplência, risco de concentração e métricas de deterioração para uma visão integrada do risco da carteira. |
| **RAROC** (Risk-Adjusted Return on Capital) | Retorno sobre o capital ajustado ao risco. Proxy calculado no modelo via ROE com ajuste de provisão. |

---

<a id="impacto-negocio"></a>

## 🎯 Impacto no Negócio

### Para o Time de Risco de Crédito
- 🔍 **Visibilidade total** sobre PD, LGD, EAD e ECL de toda a carteira, segmentada por cliente, produto e stage IFRS 9
- 📋 **Conformidade IFRS 9** com staging automático, ECL 12M e Lifetime e Migration Rates em tempo real
- 🚨 **Alertas antecipados** via EWS — detecta deterioração antes que o risco se materialize no NPL
- 📊 **Roll Rates e Vintage** para calibração de modelos internos de PD e revisão de políticas de concessão

### Para o Time de BI / Analytics
- ⚡ **+170 métricas prontas** e reutilizáveis em qualquer visual, sem reconstrução de lógica
- 🔄 **Parâmetro de métricas** — qualquer análise comparativa configurável em minutos, pelo próprio usuário
- 📅 **Parâmetro de período** — janelas temporais flexíveis sem necessidade de alterar o modelo
- 📖 **Glossário embutido** com 127 definições acessíveis diretamente no Power BI

### Para a Gestão / Diretoria
- 📊 **Visão única** de portfólio, risco, concentração e performance em um só ambiente analítico
- 🧪 **Simulação de cenários adversos** para decisões informadas de capital, provisão e apetite de risco
- 📈 **Análise histórica completa** com vintage e evolução de todos os indicadores estratégicos
- 🏛️ **Linguagem regulatória** — métricas alinhadas ao IFRS 9 e Basileia III para comunicação com órgãos supervisores

---

<a id="tecnologias"></a>

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Versão | Justificativa |
|---|---|---|
| **Power BI Desktop** | Mais recente | Plataforma de BI com engine DAX nativa, Star Schema, interatividade avançada e publicação corporativa via Power BI Service |
| **DAX** | — | Linguagem de cálculo para todas as 137 medidas — de agregações simples a índices compostos, correlações e simulações dinâmicas |
| **Power Query (M)** | — | Transformação, tipagem e preparação dos dados na camada de ingestão — antes de qualquer cálculo DAX |
| **Bookmarks + Parâmetros** | — | Interatividade avançada: agrupamentos dinâmicos, simulação de stress e comparativos temporais configuráveis pelo usuário |
| **Excel** | — | Fonte de dados estruturada com 3 tabelas de fato e 4 dimensões — `Base_Credito_Risco_2025.xlsx` |
| **IFRS 9** | CMN 4.966/2021 | Norma contábil implementada integralmente: Staging, ECL 12M e Lifetime, PD/LGD/EAD, Migration Rates |
| **Basileia III** | BIS Framework | Capital regulatório calculado sobre o EAD ponderado pelo risco da carteira (alíquota 11%) |

---

<a id="como-utilizar"></a>

## 🔧 Como Utilizar

### Pré-requisitos

- Power BI Desktop (versão mais recente recomendada)
- Arquivo `Base_Credito_Risco_2025.xlsx` disponível localmente

### Passo 1 — Clonar o repositório

```bash
git clone https://github.com/Henri-fernandes/PBI-Credit-Risk.git
cd PBI-Credit-Risk
```

### Passo 2 — Configurar a fonte de dados

Após abrir o arquivo `.pbix`:

1. Acesse **Transformar Dados → Configurações da Fonte de Dados**
2. Localize o arquivo `Base_Credito_Risco_2025.xlsx`
3. Atualize o caminho para o diretório local onde o arquivo está salvo
4. Clique em **Fechar e Aplicar**

### Passo 3 — Atualizar os dados

Clique em **Atualizar** na faixa de opções Home. As 3 tabelas de fato e as 4 dimensões serão carregadas automaticamente.

### Passo 4 — Explorar os módulos e parâmetros

Navegue pelas abas do relatório:

- Use o **seletor de métricas** para configurar as colunas da tabela analítica
- Use o **seletor de período** para escolher a janela de comparação histórica
- Use os **botões de bookmark** para alternar os agrupamentos nos gráficos
- No **Stress Test**, ajuste o parâmetro de PD para simular cenários adversos

> ⚠️ Os nomes das abas no Excel devem corresponder exatamente a: `FATO_CARTEIRA`, `FATO_RISCO`, `FATO_PROVISAO`, `DIM_CLIENTE`, `DIM_PRODUTO`, `DIM_RATING`, `DIM_TEMPO`.

---

<a id="contato"></a>

## 📧 Contato

**Henrico Fernandes**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/henricofernandes/)
[![Portfólio](https://img.shields.io/badge/Portfólio-000000?style=for-the-badge&logo=github&logoColor=white)](https://henri-fernandes.github.io/Portfolio/)
