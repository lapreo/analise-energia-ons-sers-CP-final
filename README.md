# Análise de Dados de Energia — SERS

RM: 561975 Rafael Laprega Gontijo Magalhães

**Curso:** Ciência da Computação
**Disciplina:** Soluções em Energias Renováveis e Sustentáveis (SERS)
**Professor:** André Tritiack
**Atividade:** Checkpoint 01 — Análise de Dados de Energia

## Descrição da atividade

Este repositório reúne as duas entregas da atividade prática de análise de dados do setor de energia, desenvolvidas ao longo das Aulas 03, 04 e no Desafio Final da disciplina:

1. **Exercícios das Aulas 03 e 04** — preparação e análise exploratória do Dataset 4 (Solar Power Generation Data) utilizando Orange Data Mining (inspeção, seleção de atributos, amostragem) e Python/Pandas (organização dos dados, cálculo de indicadores, criação de recortes por critério e interpretação dos resultados).
2. **Desafio Final** — análise da carga elétrica verificada da área de São Paulo (SP), obtida diretamente da API pública de Carga Verificada do Operador Nacional do Sistema Elétrico (ONS), incluindo construção do DataFrame, cálculo de indicadores, identificação de períodos de alta demanda, visualizações e relatório técnico final.

## Fontes dos dados analisados

| Etapa | Dataset | Fonte |
| --- | --- | --- |
| Exercícios Aulas 03/04 | Solar Power Generation Data (Plant 1) | [Kaggle — anikannal/solar-power-generation-data](https://www.kaggle.com/datasets/anikannal/solar-power-generation-data) |
| Desafio Final | Carga de Energia Verificada (área SP, 01/08/2025 a 07/08/2025) | [Portal de Dados Abertos do ONS](https://dados.ons.org.br/dataset/carga-energia-verificada) — API: `https://apicarga.ons.org.br/prd/cargaverificada` |

## Estrutura do repositório

```
.
├── README.md
├── exercicios/
│   └── Exercicios_Aula03_04_Dataset4_Solar.ipynb
├── desafio_final/
│   └── Desafio_Final_Energia_ONS_API.ipynb
└── orange/
    ├── FLUXO_BASE.ows
    └── amostra_solar_plant.tab
```

- **`exercicios/`** — notebook com a resolução dos exercícios das Aulas 03 e 04 (Dataset 4 — Solar Power Generation Data), com a etapa do Orange Data Mining documentada e o código Python/Pandas executado, incluindo inspeção inicial, renomeação de atributos, cálculo do limiar de alta geração e identificação do inversor mais frequente nos registros de alta geração.
- **`desafio_final/`** — notebook do Desafio Final, com a consulta à API do ONS, construção e organização do DataFrame, cálculo de indicadores (carga mínima, máxima, média, mediana), identificação de períodos de alta demanda, visualizações, síntese dos resultados e relatório técnico final elaborado pela equipe.
- **`orange/`** — fluxo de trabalho do Orange Data Mining (`FLUXO_BASE.ows`) e a amostra de dados exportada (`amostra_solar_plant.tab`, formato nativo do Orange), utilizada como entrada do notebook de exercícios.

## Como executar

Os notebooks foram desenvolvidos para rodar no **Google Colab**, pois a etapa do Desafio Final depende de acesso à internet (consulta à API do ONS).

1. Abra o notebook desejado no Google Colab (`Arquivo > Fazer upload de notebook`).
2. Faça upload do arquivo de dados correspondente (`amostra_solar_plant.tab`, na pasta `orange/`) para a sessão do Colab, através do painel de arquivos lateral.
3. Execute as células em ordem, do início ao fim.

## Integrantes do grupo

*(Preencher com os nomes dos integrantes da equipe.)*
