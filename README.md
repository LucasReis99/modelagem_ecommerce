# Desafio de Modelagem de Dados

## Descrição do Projeto
Este projeto apresenta um modelo de banco de dados desenvolvido para gerenciar um sistema de pedidos e pagamentos, incluindo detalhes sobre clientes, pagamentos, e entregas. O objetivo foi criar um modelo claro e eficaz que atenda aos requisitos de um sistema de e-commerce.

## Estrutura do Modelo

### Entidades Principais
#### Cliente: Representa tanto clientes Pessoa Física (PF) quanto Pessoa Jurídica (PJ). A diferenciação entre PF e PJ é feita através das tabelas específicas ClientePF e ClientePJ, eliminando a necessidade de um campo Tipo na tabela Cliente.

#### Pagamento: Associa-se aos pedidos e pode ter múltiplas formas de pagamento. Utiliza o tipo DECIMAL para armazenar valores monetários de forma precisa.

#### Entrega: Gerencia o status e o código de rastreio das entregas associadas aos pedidos. A tabela Entrega foi adicionada para garantir o rastreamento e a gestão eficiente das entregas.

### Tabelas e Relacionamentos

#### Cliente: Base para ClientePF e ClientePJ. Não possui o campo Tipo por conta da herança de tabelas.

#### Pedido: Associado a clientes e pagamentos, e gerencia o estado dos pedidos.

#### Pagamento: Relacionado a pedidos com a possibilidade de múltiplas formas de pagamento.

#### Entrega: Relacionada a pedidos e inclui atributos como status, prazo, e código de rastreio.

## Implementação

As tabelas e seus relacionamentos foram cuidadosamente planejados para atender aos requisitos funcionais e garantir a integridade dos dados.

## Objetivo do Desafio

O desafio consistiu em refinar o modelo de dados para incluir a diferenciação entre Pessoa Física e Jurídica, permitir múltiplas formas de pagamento, e adicionar a tabela de Entrega com os atributos necessários para rastreamento e status. O projeto foi adicionado ao GitHub para futura avaliação e está disponível para consulta e feedback.

## Instruções
Para visualizar o diagrama completo, consulte o arquivo Diagrama.png.
Para detalhes sobre a implementação, consulte os scripts SQL na pasta scripts.
