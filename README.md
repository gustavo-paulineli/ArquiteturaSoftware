# Projeto TechStore — Refatoração Orientada a Objetos & SOLID

Este repositório contém a versão refatorada e corrigida do sistema **TechStore**, referente à atividade de diagnóstico de Arquitetura de Software.

## 🚀 Melhorias Aplicadas
- **SRP (Single Responsibility Principle):** Divisão de `OrderService` em componentes especializados (`OrderValidator`, `DiscountCalculator`, `FreightCalculator`, `PaymentProcessor`).
- **OCP (Open/Closed Principle):** Estratégia extensível para taxas de frete e regras de desconto sem modificação da classe principal.
- **DIP (Dependency Inversion Principle):** Injeção de dependências no construtor de `OrderService`.
- **Princípio de Demeter:** Encapsulamento de chamadas profundas (`customer.getRegion()`, `order.getTotalWeight()`).
- **Testes Automatizados:** Suíte de testes criada com o test runner nativo do Node.js (`node --test`).

## 🛠️ Como Executar

### Requisitos
- Node.js v20 ou superior.

### Executar a aplicação
```bash
npm start
```

### Executar os testes automatizados
```bash
npm test
```
