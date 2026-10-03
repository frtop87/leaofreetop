# 🦁 Leão Freetop — Organizador de Dados para o Imposto de Renda em Excel

> Planilha em Excel que ajuda a **organizar e reunir, em um só lugar, as informações essenciais para a declaração de Imposto de Renda (IRPF)**.
> Projeto desenvolvido na plataforma **DIO** em parceria com o **Santander**.

![Excel](https://img.shields.io/badge/Excel-217346?logo=microsoftexcel&logoColor=white)
![DIO](https://img.shields.io/badge/DIO-Bootcamp-blue)
![Status](https://img.shields.io/badge/status-concluído-brightgreen)

---

## 📑 Sumário

1. [Sobre o projeto](#-sobre-o-projeto)
2. [Problema e objetivo](#-problema-e-objetivo)
3. [Estrutura do repositório](#-estrutura-do-repositório)
4. [Estrutura da planilha](#-estrutura-da-planilha)
5. [Capturas de tela](#-capturas-de-tela)
6. [Como usar](#-como-usar)
7. [Recursos do Excel utilizados](#-recursos-do-excel-utilizados)
8. [Aprendizados](#-aprendizados)
9. [Melhorias futuras](#-melhorias-futuras)
10. [Aviso importante](#-aviso-importante)
11. [Autor](#-autor)

---

## 📌 Sobre o projeto

O **Freetop IR** é uma ferramenta de apoio ao contribuinte pessoa física. Na época da declaração do Imposto de Renda, é comum ter documentos e valores espalhados: informes de rendimentos de vários bancos, extratos, holerites, notas e comprovantes. A planilha centraliza esses dados em três etapas simples, com navegação por botões, para que na hora de declarar tudo esteja organizado e conferido.

## 🎯 Problema e objetivo

**Problema:** informações dispersas dificultam o preenchimento da declaração e aumentam o risco de esquecimentos e erros (e, consequentemente, de cair na malha fina).

**Objetivo:** oferecer uma planilha visual, guiada e fácil de preencher que:

- reúna os **dados cadastrais do titular**;
- consolide os **informes de rendimentos bancários** e calcule o total;
- registre as **entradas** (notas bancárias, extratos ou holerites) com data, categoria e valor;
- sirva de base de consulta no momento de preencher o programa da Receita Federal.

## 🗂️ Estrutura do repositório

```text
leaofreetop/
├── README.md                  # Documentação principal (este arquivo)
├── planilha/
│   └── Freetop_IR.xlsx        # Arquivo Excel do projeto (adicionar)
├── images/
│   ├── 01-aba-titular.png     # Captura da aba TITULAR
│   ├── 02-aba-informes.png    # Captura da aba INFORMES
│   └── 03-aba-notas.png       # Captura da aba NOTAS
└── docs/
    ├── guia-de-uso.md         # Passo a passo de preenchimento
    └── estrutura-da-planilha.md  # Detalhamento de campos e abas
```

## 🧩 Estrutura da planilha

A planilha é dividida em **três seções**, acessadas pelo menu lateral (TITULAR, INFORMES e NOTAS). Em cada tela, os botões **PRÓXIMO ->** e **<- ANTERIOR** permitem avançar ou voltar entre as etapas. Células em amarelo indicam campos de preenchimento.

### 1. Dados do Titular

Cadastro da pessoa física que vai declarar:

| Campo | Descrição |
|---|---|
| Nome | Nome completo do contribuinte |
| CPF | Cadastro de Pessoa Física |
| Nascimento | Data de nascimento |
| Título de eleitor | Número do título |
| Cônjuge | Nome do cônjuge, se houver |
| Rua / Rua abreviada | Endereço completo e versão abreviada |
| CEP | Código postal |
| Telefone / Celular | Contatos |
| E-mail | Contato eletrônico |
| Houve alterações da entrega anterior | SIM/NÃO |
| Dependente cônjuge | SIM/NÃO |
| Residente do exterior | SIM/NÃO |

### 2. Informe de Rendimentos Bancários

Registro, por instituição financeira, do saldo/valor atual informado nos informes de rendimentos:

| Campo | Descrição |
|---|---|
| **Total** | Soma automática dos valores de todos os bancos |
| Banco | Código e nome da instituição (ex.: `33 - Banco Santander`) |
| Valor atual | Valor em R$ informado pelo banco |
| Anexo | Referência ao documento/informe correspondente |

### 3. Notas Bancárias ou Extrato de Holerites

Tabela de **Entradas** para lançar os recebimentos ao longo do ano:

| Coluna | Descrição |
|---|---|
| Data | Data do recebimento |
| Categoria | Origem da entrada (ex.: `CNPJ`) |
| Valor | Valor em R$ |

A tabela possui **filtros** em cada coluna, o que facilita ordenar, buscar e conferir os lançamentos.

## 🖼️ Capturas de tela

### Aba Titular
![Aba Titular](images/01-aba-titular.png)

### Aba Informes
![Aba Informes](images/02-aba-informes.png)

### Aba Notas
![Aba Notas](images/03-aba-notas.png)

> ⚠️ Todos os dados exibidos nas imagens são **fictícios**, usados apenas para demonstração.

## ▶️ Como usar

1. Baixe o arquivo em [`planilha/Freetop_IR.xlsx`](planilha/).
2. Abra no **Microsoft Excel** (recomendado: versão 2016 ou superior) e, se solicitado, clique em **Habilitar edição**.
3. Em **TITULAR**, preencha os campos amarelos e clique em **PRÓXIMO ->**.
4. Em **INFORMES**, informe cada banco, o valor atual e o anexo; confira o **Total**.
5. Em **NOTAS**, lance cada entrada com data, categoria e valor.
6. Use os dados consolidados como apoio ao preencher a declaração no programa oficial da Receita Federal.

Mais detalhes em [`docs/guia-de-uso.md`](docs/guia-de-uso.md).

## 🛠️ Recursos do Excel utilizados

- Layout personalizado com **menu lateral de navegação**
- **Botões com hiperlinks** entre abas e células (PRÓXIMO / ANTERIOR)
- **Tabelas formatadas** com filtros
- **Fórmulas** para somatório automático dos valores
- **Formatação de moeda** (R$) e de datas
- **Formatação visual** com cores para destacar campos de preenchimento
- Campos de seleção (SIM/NÃO) e categorias *(ajuste conforme a validação de dados usada)*

## 📚 Aprendizados

- Estruturação de uma planilha como se fosse um pequeno sistema, pensando na experiência de quem preenche
- Uso de navegação e organização visual para reduzir erros de digitação
- Consolidação de dados financeiros de várias fontes
- Documentação de projeto e publicação no GitHub para portfólio

## 🚀 Melhorias futuras

- Incluir aba de **despesas dedutíveis** (saúde, educação, previdência)
- Incluir aba de **bens e direitos** e **dívidas**
- Adicionar **dashboard** com resumo e gráficos
- Validação de CPF e CEP
- Versão para Google Planilhas

## ⚖️ Aviso importante

Esta ferramenta é apenas um **organizador de informações**, com fins educacionais. Ela **não substitui** o programa oficial da Receita Federal nem a orientação de um contador. Confira sempre os valores com os documentos originais.

## 👤 Autor

**Frizzo** — [@frtop87](https://github.com/frtop87)

Projeto desenvolvido no bootcamp da [DIO](https://www.dio.me/) em parceria com o **Santander**.
