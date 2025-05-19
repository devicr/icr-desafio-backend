# Desafio Back-end ICR

Primeiramente, obrigado pelo seu interesse em trabalhar conosco!
Abaixo você encontrará todos as informações necessárias para iniciar o seu teste.

## Avisos antes de começar

- Leia com atenção este documento por completo e tente seguir ao **máximo** as instruções;
- Crie um repositório no seu GitHub **sem citar nada relacionado à ICR**;
- Faça seus commits normalmente no seu repositório;
- Envie o link do repositório para o e-mail ou número do **recrutador responsável** (por número há tendência de resposta mais rápida);
- Você poderá consultar o Google, Stack Overflow, IAs ou algum projeto pessoal salvo localmente;
- Fique à vontade para tirar dúvidas com os recrutadores;
- Fique tranquilo, respire — não tem problema não saber tudo, o importante é tentar. Boa sorte! 😊


_Corpo do Email ou Mensagem com o link do repositório do desafio_

> Seu Nome
>
> Link do repositório
>

### Sobre o ambiente da aplicação:

- Utilize o **Spring Boot** como framework principal para a implementação deste desafio.

- Fique à vontade para utilizar a **IDE de sua preferência**.

> Valorizamos uma boa estrutura de containeres criada por você.

## Objetivo: Seguro Auto Simplificado

O Seguro Auto Simplificado é uma plataforma de simulação de seguros de automóveis. 
Nela é possível cadastrar clientes e veículos, e realizar cotações com base em regras de negócio típicas do setor de seguros.

### Requisitos

A seguir estão as regras de negócio que devem ser consideradas no sistema:

- O sistema deve receber os seguintes dados:
  - `nome` do condutor
  - `idade` do condutor
  - `modelo` do veículo
  - `ano_fabricacao` do veículo
  - `cidade_residencia` do condutor
  - `historico_sinistro` (booleano: true/false)

- O valor base do seguro é de **R$ 1.000,00**

- Regras de cálculo:

  - **Idade do condutor**:
    - Menor que 25 anos → acréscimo de 20%
    - De 25 a 60 anos → sem alteração
    - Acima de 60 anos → acréscimo de 15%

  - **Ano de fabricação do veículo**:
    - Se o veículo tem mais de 10 anos → acréscimo de 10%

  - **Histórico de sinistro**:
    - Se verdadeiro (já teve sinistro) → acréscimo de 25%

  - **Cidade de residência**:
    - Se for `São Paulo` → acréscimo de 10%
    - Se for `Curitiba` → desconto de 5%
    - Qualquer outra → sem alteração

- A resposta da API deve conter o **valor final da cotação** e um **resumo dos critérios aplicados**.
- O serviço deve ser **RESTful**.

## 🧪 Exemplo de requisição

```http
POST /cotacoes
Content-Type: application/json

{
  "nome": "João Silva",
  "idade": 22,
  "modelo": "Fiat Uno",
  "ano_fabricacao": 2005,
  "cidade_residencia": "São Paulo",
  "historico_sinistro": true
}
```

Caso ache interessante, faça uma **proposta** de endpoint e apresente para os entrevistadores :heart:

## O que será avaliado e valorizamos :heart:

Habilidades básicas de criação de projetos backend:
- Conhecimentos sobre REST
- Uso do Git e Lombok
- Capacidade analítica
- Apresentação de código limpo e organizado

Conhecimentos intermediários de construção de projetos manuteníveis:
- Aplicação e conhecimentos de SOLID
- Identificação e aplicação de Design Patterns
- Conhecimentos sobre conceitos de containers (Docker)
- Documentação e descrição de funcionalidades e manuseio do projeto
- Implementação e conhecimentos sobre testes de unidade e integração
- Identificar e propor melhorias
- Boas noções de bancos de dados relacionais

## O que NÃO será avaliado :warning:

- Frontend, só avaliaremos a API Restful
- Autenticação

## O que será um Diferencial

- Uso de Docker
- Uma cobertura de testes consistente
- Uso de Design Patterns
- Documentação
- Proposta de melhoria na arquitetura
- Ser consistente e saber argumentar suas escolhas
- Apresentar soluções que domina
- Modelagem de Dados
- Manutenibilidade do Código
- Tratamento de erros
- Cuidado com itens de segurança
- Arquitetura (estruturar o pensamento antes de escrever)
- Carinho em desacoplar componentes (outras camadas, service, repository)  
