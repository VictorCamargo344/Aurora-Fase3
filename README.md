# Sistema Inteligente de Gerenciamento Energético da Colônia Aurora Siger (SIGER-3)

## Equipe
- Lucas Araujo de Carvalho
- Pietra Fanticelli
- Rafael Gonçalves de Souza Pereira
- Victor de Camargo Gomes

## Descrição do Projeto

O projeto SIGER-3 (Sistema Inteligente de Gerenciamento Energético e Resposta da Colônia) foi desenvolvido com o objetivo de representar o funcionamento inteligente da colônia fictícia Aurora Siger, localizada em Marte, na região de Hellas Planitia.

O sistema integra conceitos estudados ao longo da disciplina, como:

- Estruturas de dados;
- Organização hierárquica;
- Lógica de programação;
- Tomada de decisão automatizada;
- Regressão linear simples;
- Análise energética;
- Sistemas preditivos.

A aplicação foi desenvolvida em Python e simula o gerenciamento energético da colônia, monitorando geração solar e eólica, consumo energético, reserva de energia, condições ambientais e prioridade dos módulos operacionais.

---
## Estrutura do Repositório 

```
siger3/
├── .gitignore         # Arquivos e pastas ignorados pelo Git
├── README.md          # Documentação principal do projeto
├── script.ipynb       # Notebook com o código do sistema SIGER-3
└── relatorio.pdf      # Relatório explicativo do projeto
```

# Objetivos do Sistema

O sistema foi desenvolvido para:

- Organizar os dados da colônia em estruturas hierárquicas;
- Monitorar geração e consumo de energia;
- Automatizar decisões energéticas;
- Priorizar sistemas essenciais;
- Detectar cenários críticos;
- Gerar alertas operacionais;
- Prever geração eólica utilizando regressão linear;
- Evoluir de um sistema reativo para um sistema preditivo.

---

# Estrutura da Colônia

A colônia foi organizada em três grandes sistemas:

## Sistema Energético

Responsável pelo gerenciamento da geração e reserva de energia.

### Subsistemas

- Energia solar;
- Energia eólica;
- Reserva energética.

---

## Sistema Ambiental

Responsável pelo monitoramento das condições ambientais marcianas.

### Sensores

- Temperatura interna;
- Temperatura externa;
- Velocidade do vento;
- Pressão atmosférica;
- Radiação solar.

---

## Sistema Operacional

Responsável pelos módulos ativos da colônia.

### Módulos

- Habitat Alpha;
- MedBase;
- Reator Solar;
- BioLab;
- LogiStore;
- TerraBot.

Cada módulo possui:

- prioridade;
- consumo energético;
- status operacional.

---

# Tecnologias e Conceitos Utilizados

- Python 3;
- Funções e modularização;
- Estruturas de dados com listas e dicionários;
- Organização hierárquica;
- Lógica condicional;
- Regressão linear simples;
- Método dos mínimos quadrados;
- Simulação de cenários operacionais.

---

# Funcionalidades do Sistema

## Organização Hierárquica

Os dados da colônia foram estruturados utilizando dicionários aninhados, permitindo representar sistemas e subsistemas de forma organizada.

---

## Leitura de Sensores

O sistema realiza leitura e resumo das informações ambientais e energéticas da colônia.

---

## Cálculo Energético

O sistema calcula:

- geração total de energia;
- consumo total dos módulos;
- saldo energético;
- nível de reserva.

---

## Priorização de Sistemas

Os módulos são organizados por prioridade, garantindo que sistemas essenciais sejam preservados em situações críticas.

---

## Motor de Decisão Inteligente

O sistema aplica regras automáticas para tomada de decisão.

### Exemplos

- Se consumo > geração → ALERTA;
- Se reserva < 20% → estado CRÍTICO;
- Se geração muito acima do consumo → estado EFICIENTE;
- Se vento extremo → recolher painéis solares;
- Se temperatura externa crítica → verificar isolamento térmico.

---

## Regressão Linear

Foi implementado um modelo de regressão linear simples para prever geração de energia eólica com base na velocidade do vento.

### Fórmula
```python
Energia = m * vento + b
```

## Limites Operacionais da Turbina

O sistema considera limites reais de funcionamento da turbina eólica:

- Cut-in → velocidade mínima para operar;
- Potência nominal → geração máxima;
- Cut-out → desligamento por segurança em ventos extremos.

---

## Cenários Simulados

O sistema executa diferentes cenários operacionais:

### Operação Normal

Geração maior que consumo.

---

### Alerta de Consumo

Consumo maior que geração.

---

### Situação Crítica

Consumo maior que geração e reserva baixa.

---

### Operação Eficiente

Grande excedente energético.

---

### Tempestade Marciana

Ventos extremos e temperatura crítica.

---

### Modo Economia

Desligamento de módulos menos prioritários.

---

## Exemplo de Entrada

```python
geracao = 40
consumo = 70
reserva_pct = 60
temp_ext = -63
vento = 15
```
## Exemplo de Saída
```python 
STATUS: ALERTA

Alertas:
-> Consumo maior que geração

Ações recomendadas:
* Ativar modo economia
* Reduzir consumo de TerraBot e LogiStore
```

## Objetivo Acadêmico

O projeto foi desenvolvido com o objetivo de integrar os conteúdos estudados ao longo da disciplina em uma solução computacional única, demonstrando como lógica, estruturas de dados e modelagem matemática podem ser utilizadas para criar sistemas inteligentes capazes de monitorar, prever e otimizar recursos energéticos.

# Integrantes 
- Victor de Camargo Gomes:
  victor.camargog24@gmail.com

- Pietra Fanticelli:
pf.pietrafanticelli@gmail.com

- Rafael Gonçalves de Souza Pereira:
rafagonpereira12@gmail.com
