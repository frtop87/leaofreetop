# Arquitetura conceitual

## Objetivo

A experiência documentada segue um modelo de formulário dividido em etapas. A divisão reduz a quantidade de informação apresentada simultaneamente e permite ao usuário avançar e retornar entre seções.

## Componentes

### 1. Titular

Responsável por concentrar informações cadastrais:

- nome;
- CPF;
- nascimento;
- título de eleitor;
- cônjuge;
- endereço;
- telefone;
- celular;
- e-mail;
- indicadores complementares.

### 2. Informações bancárias

Responsável por organizar informações por instituição:

- banco/instituição;
- valor atual;
- referência a anexo/comprovante;
- total consolidado.

### 3. Navegação

O fluxo visual utiliza ações equivalentes a:

- `PRÓXIMO` para avançar;
- `ANTERIOR` para retornar.

## Modelo conceitual

```mermaid
flowchart LR
    A[Dados do titular] --> B[Informações bancárias]
    B --> C[Notas / demais informações]

    A --> D[Validação]
    B --> D
    C --> D

    D --> E[Persistência segura]
    E --> F[Relatório / exportação]
```

## Requisitos funcionais sugeridos

| ID | Requisito |
|---|---|
| RF-01 | Permitir preenchimento dos dados do titular |
| RF-02 | Permitir cadastro de múltiplas instituições |
| RF-03 | Calcular/consolidar o total informado |
| RF-04 | Permitir navegação entre etapas |
| RF-05 | Permitir associação de comprovantes |
| RF-06 | Validar dados antes da conclusão |
| RF-07 | Registrar alterações relevantes |
| RF-08 | Permitir geração de relatório |

## Requisitos não funcionais sugeridos

- proteção de dados pessoais;
- autenticação e autorização;
- criptografia em trânsito e em repouso;
- logs sem exposição de dados sensíveis;
- backups protegidos;
- controle de acesso baseado em função;
- validação no cliente e no servidor;
- tratamento seguro de uploads;
- testes automatizados.
