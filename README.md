# FlexOrder-DesignPatterns
Aula_Ale_09
## 📚 Explicação do projeto

Este projeto implementa um sistema de checkout utilizando **Programação Orientada a Objetos (POO)** e padrões de projeto, simulando um fluxo completo de compra com pagamento, frete, estoque e emissão de nota.

---

### 🔹 Estratégia de pagamento e frete (Strategy Pattern)

O sistema utiliza o padrão **Strategy**, permitindo definir diferentes formas de pagamento e tipos de frete de forma flexível.

- Pagamentos disponíveis:
  - Cartão de crédito
  - PIX
  - Transferência alternativa (Mana)

- Tipos de frete:
  - Normal
  - Expresso
  - Teletransporte

Cada estratégia possui sua própria lógica, podendo ser alterada sem impactar o restante do sistema.

---

### 🔹 Classe Pedido

A classe responsável por representar uma compra, contendo:

- Lista de itens  
- Método de pagamento  
- Tipo de frete  
- Cálculo de valor total  
- Aplicação de descontos  

Também realiza o cálculo final da compra somando o valor com desconto e o custo do frete.

---

### 🔹 Regras de negócio

O sistema aplica regras como:

- Desconto para pagamentos via PIX  
- Desconto para pedidos com valor elevado  
- Cálculo dinâmico de frete  

---

### 🔹 Controle de estoque

O sistema verifica a disponibilidade dos itens antes de concluir a compra.

Caso não haja estoque suficiente, o processo é interrompido.

---

### 🔹 Geração de nota fiscal

Após a confirmação do pagamento, o sistema simula a emissão de uma nota fiscal com o valor final da compra.

---

### 🔹 Sistema de notificação

O cliente recebe uma confirmação do pedido após a finalização do processo.

---

### 🔹 Facade (Padrão de projeto)

O projeto utiliza o padrão **Facade**, centralizando todo o processo de checkout em uma única classe.

Essa classe coordena:

- Atualização de estoque  
- Processamento de pagamento  
- Cálculo de valores  
- Emissão de nota  
- Envio de confirmação  

---

### 🔹 Fluxo do sistema

O processo de compra segue as etapas:

1. Validação de estoque  
2. Aplicação de desconto  
3. Cálculo de frete  
4. Processamento do pagamento  
5. Emissão de nota fiscal  
6. Envio de confirmação  

---

## 🎯 Conclusão

Este projeto demonstra:

- Programação Orientada a Objetos (POO)
- Uso de classes abstratas e herança
- Padrões de projeto (Strategy e Facade)
- Separação de responsabilidades
- Simulação de regras de negócio reais
- Organização de código em sistemas complexos
