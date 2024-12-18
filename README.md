# Projeto E-commerce - Modelo de Banco de Dados

## Descrição
Este repositório contém o modelo conceitual básico de um banco de dados para um sistema de e-commerce, desenvolvido utilizando o MySQL Workbench. O modelo define as entidades, atributos e relacionamentos necessários para representar as informações de produtos, clientes, pedidos e outras informações relevantes para um e-commerce.

## Tecnologias Utilizadas
* **MySQL Workbench:** Ferramenta utilizada para modelar o banco de dados.
* **MySQL:** Sistema gerenciador de banco de dados relacional.

## Estrutura do Projeto
* **e-commerce.mwb:** Arquivo principal do projeto, contendo o diagrama ER (Entidade-Relacionamento) completo.
* **e-commerce.png:** O diagrama do Projeto Coneceitual modelado.

## Como Utilizar
1. **Importar o modelo:** Abra o arquivo `e-commerce.mwb` no MySQL Workbench.
2. **Conectar ao banco de dados:** Configure a conexão com o seu banco de dados MySQL.
3. **Gerar script SQL:** Utilize a função de geração de script SQL do Workbench para criar o script de criação das tabelas e índices.
4. **Executar o script:** Execute o script SQL gerado no seu banco de dados MySQL.

## Contribuições
Contribuições são bem-vindas! Abra um issue ou um pull request para propor melhorias ou correções.

## Documentação
## Objetivo do Banco de Dados

* Armazenar informações sobre produtos, clientes, pedidos, fornecedores, estoque e pagamentos de um e-commerce.
* Gerenciar o processo de venda, desde a escolha do produto até a entrega.

## Descrição das Tabelas

* **Fornecedor:**
    * Armazena os dados cadastrais dos fornecedores da plataforma.
* **Produto:**
    * Armazena as informações dos produtos, incluindo categoria, descrição e valor.
* **Cliente:**
    * Armazena os dados cadastrais dos clientes, diferenciando pessoas físicas e jurídicas. Um mesmmo cliente não pode ter registrado, na mesma conta, CPF e CNPJ. Dessa forma, ele deve ter uma conta para cada identificação (PF ou PJ).
* **Pedido:**
    * Armazena os dados dos pedidos realizados pelos clientes, incluindo status, valor total e informações de entrega.
* **Entrega:**
    * Armazena as informações sobre a entrega dos pedidos, como status e código de rastreio.
* **Estoque:**
    * Armazena as informações sobre a quantidade de produtos em estoque em diferentes locais.
* **Terceiro Vendedor:**
    * Armazena os dados cadastrais de terceiros vendedores que fornecem produtos.
* **Produtos por Terceiros:**
    * Relaciona os produtos com os terceiros vendedores.
* **Relação de Produto por Pedido:**
    * Detalha os produtos incluídos em cada pedido e suas respectivas quantidades.
* **Cartão de Pagamento:**
    * Armazena as informações dos cartões de pagamento utilizados pelos clientes. Um mesmo cliente pode registrar mais de um cartão para pagamento. Não foram incluídos opções para pagamento em boleto ou PIX.

## Licença
Este projeto está licenciado sob a MIT License.

![e-commerce](https://github.com/user-attachments/assets/65ddba37-188c-40f9-b5e8-097b37d4f5d7)
