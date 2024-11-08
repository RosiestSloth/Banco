# Projeto Banco

Este é um projeto Java simples que simula operações bancárias básicas. Ele permite a criação de contas, realização de operações de crédito e débito, e implementação de contas especiais com limite de cheque especial.

## Estrutura do Projeto

O projeto consiste nas seguintes classes:

- **Banco**: Classe principal que executa o programa, simulando operações em diferentes contas bancárias.
- **Conta**: Classe base que representa uma conta bancária comum, com métodos para configurar número de conta, saldo e operações de crédito e débito.
- **ContaNormal**: Subclasse de `Conta` para contas regulares.
- **ContaDebEspecial**: Subclasse de `Conta` para contas com limite de débito especial.

## Funcionalidades

- Criação de contas bancárias com número de conta e saldo inicial.
- Realização de operações de crédito e débito.
- Configuração e utilização de um limite especial para contas de débito especial.

## Exemplo de Uso

No código principal (`Banco`), o programa cria e realiza operações em duas contas de exemplo:

1. Uma **ContaNormal** com saldo inicial de R$ 500,00.
2. Uma **ContaDebEspecial** com saldo inicial de R$ 2500,00 e limite de R$ 1000,67.

### Saída Esperada

Ao executar o código principal, são exibidas as informações das operações realizadas nas contas, incluindo créditos e débitos e atualizações no saldo e limite.

Exemplo:
```plaintext
A conta número 1654-3 possui saldo 500.0
Após o crédito de R$ 1000,00, a conta número 1654-3 passou a ter saldo 1500.0
Após o débito de R$ 100,00, a conta número 1654-3 passou a ter saldo 1400.0

A conta número 4067-6 possui saldo 2500.0
Após o débito de R$ 500,00, a conta número 4067-6 passou a ter saldo 2000.0
A conta número 4067-6 possui saldo 2000.0 e limite de 10000.0
```

## Como Executar

1. Clone o repositório para sua máquina local.
2. Compile as classes Java:
   ```bash
   javac Banco.java
   ```
3. Execute o programa:
   ```bash
   java Banco
   ```

## Requisitos

- Java Development Kit (JDK) 8 ou superior.
