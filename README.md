# 🧪 Critérios de Aceitação (BDD) — Encerramento de Conta

## ✅ Cenários Positivos

### **1. Encerramento permitido**
**Dado** que o usuário não possui saldo nem débitos  
**Quando** solicita encerramento  
**Então** o sistema deve encerrar a conta.

### **2. Tentativa de acesso após encerramento**
**Dado** que o usuário encerra a conta com sucesso  
**Quando** tenta acessá-la novamente  
**Então** o sistema deve exibir a mensagem **"Conta encerrada"**.

---

## ❌ Cenários Negativos

### **3. Conta com saldo positivo**
**Dado** que o usuário possui saldo positivo  
**Quando** solicita encerramento  
**Então** o sistema deve recusar e exibir **"Conta não pode ser encerrada com saldo disponível"**.

### **4. Conta com pendências financeiras**
**Dado** que o usuário possui empréstimos ou débitos pendentes  
**Quando** solicita encerramento  
**Então** o sistema deve recusar com a mensagem **"Conta possui pendências financeiras"**.
