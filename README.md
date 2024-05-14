# Sistema Bancário 🏦

Este é um sistema bancário simples implementado em Python, que permite a criação de clientes, contas bancárias, e realização de transações como depósitos e saques.

## Funcionalidades Principais ⚒️

- **Criação de Clientes:** Permite a criação de clientes, representados pela classe `PessoaFisica`, que contém informações como nome, CPF, data de nascimento e endereço.
- **Criação de Contas Bancárias:** O sistema permite a criação de contas bancárias, representadas pela classe `ContaCorrente`, que podem ser associadas a um cliente.
- **Depósitos e Saques:** Os clientes podem realizar depósitos e saques em suas contas bancárias.
- **Exibição de Extrato:** É possível visualizar o extrato de uma conta bancária, mostrando todas as transações realizadas.

## Estrutura do Código 🧱

O código é dividido em várias classes e funções:

### Classes 📋

1. **Cliente (`Cliente`):** Representa um cliente do banco, com informações básicas como endereço e uma lista de contas associadas.
2. **Pessoa Física (`PessoaFisica`):** Subclasse de `Cliente`, representa uma pessoa física com nome, data de nascimento, CPF e endereço.
3. **Conta (`Conta`):** Representa uma conta bancária genérica, com número, saldo, agência e cliente associado.
4. **Conta Corrente (`ContaCorrente`):** Subclasse de `Conta`, representa uma conta corrente com limite de saque e limite de saldo negativo.
5. **Histórico (`Historico`):** Mantém o registro de todas as transações realizadas em uma conta.
6. **Transação (`Transacao`):** Classe abstrata representando uma transação genérica.
7. **Saque (`Saque`):** Subclasse de `Transacao`, representa uma transação de saque.
8. **Depósito (`Deposito`):** Subclasse de `Transacao`, representa uma transação de depósito.

### Funções ⚙️

1. **Menu (`menu()`):** Exibe um menu de opções para o usuário interagir com o sistema.
2. **Filtrar Cliente (`filtrar_cliente(cpf, clientes)`):** Filtra um cliente pelo CPF na lista de clientes.
3. **Recuperar Conta Cliente (`recuperar_conta_cliente(cliente)`):** Recupera a conta de um cliente (atualmente retorna apenas a primeira conta associada ao cliente).
4. **Depositar (`depositar(clientes)`):** Permite que um cliente realize um depósito em sua conta.
5. **Sacar (`sacar(clientes)`):** Permite que um cliente realize um saque de sua conta.
6. **Exibir Extrato (`exibir_extrato(clientes)`):** Exibe o extrato de transações de uma conta bancária.
7. **Criar Cliente (`criar_cliente(clientes)`):** Permite a criação de um novo cliente.
8. **Criar Conta (`criar_conta(numero_conta, clientes, contas)`):** Permite a criação de uma nova conta bancária associada a um cliente.
9. **Listar Contas (`listar_contas(contas)`):** Lista todas as contas bancárias criadas no sistema.
10. **Main (`main()`):** Função principal que controla o fluxo do programa.

## Como Usar ▶️

Para utilizar o sistema, execute o arquivo `main.py`. Isso iniciará a interação com o sistema bancário, onde você poderá escolher diversas opções do menu para criar clientes, contas bancárias, realizar transações e visualizar extratos.

## Contribuições 💬

Contribuições são bem-vindas! Se você encontrar algum problema, bug ou tiver alguma melhoria a sugerir, sinta-se à vontade para abrir uma issue ou enviar um pull request.
