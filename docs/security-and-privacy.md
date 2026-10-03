# Segurança e privacidade

## Regra principal

Este repositório é público. Portanto, **não publique informações pessoais, financeiras ou documentos reais**.

As capturas de tela disponíveis em `/images` foram sanitizadas antes da publicação.

## Informações que devem ser removidas ou mascaradas

- CPF;
- RG e outros documentos;
- endereço residencial;
- telefone e celular;
- e-mail pessoal;
- título de eleitor;
- dados bancários;
- saldos e valores patrimoniais;
- comprovantes;
- documentos anexados;
- tokens, senhas e chaves de API;
- identificadores internos;
- informações que permitam correlacionar uma pessoa com seu patrimônio.

## Dados financeiros

Valores financeiros devem ser substituídos por dados fictícios quando a finalidade for demonstrar somente a interface.

Exemplo:

```text
Valor real:        NÃO PUBLICAR
Valor demonstrativo: R$ 10.000,00
```

## Arquivos e anexos

Antes de publicar qualquer arquivo:

1. verificar o conteúdo;
2. remover metadados quando necessário;
3. confirmar que não há documentos incorporados;
4. procurar credenciais e tokens;
5. revisar nomes, caminhos e identificadores;
6. confirmar que os exemplos são fictícios.

## Recursos do GitHub

Para repositórios públicos, o GitHub recomenda habilitar mecanismos de segurança disponíveis, incluindo alertas do Dependabot, secret scanning, push protection e code scanning quando aplicáveis.

## Checklist pré-publicação

- [x] Capturas de tela sanitizadas
- [x] Dados pessoais removidos das imagens públicas
- [x] Valores financeiros removidos das imagens públicas
- [x] README criado
- [x] Documentação de arquitetura criada
- [x] Orientações de privacidade criadas
- [ ] Revisão final no GitHub
- [ ] Ativação das proteções de segurança do repositório
