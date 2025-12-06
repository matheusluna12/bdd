## Ativ. SO - BDD

## Encerramento de Conta

**Como** cliente do banco  
**Quero** transferir dinheiro entre minhas contas ou para outra conta  
**Para** pagar minhas contas e realizar pagamentos do dia a dia.

---

## Descrição

O sistema deve permitir que um cliente autenticado selecione uma conta de origem, informe a conta de destino e o valor da transferência.  
O sistema valida:

- Se há saldo suficiente  
- Se a conta de destino existe  

Em caso de sucesso:

- Debita o valor da conta de origem  
- Credita o valor da conta de destino  
- Registra a operação com data/hora

---

## Critérios de aceitação

- A transferência só pode ocorrer se o cliente estiver **autenticado**.
- O sistema **não deve permitir** transferências com **saldo insuficiente**.
- O sistema **não deve permitir** transferências para **conta inexistente**.

### Em caso de sucesso, o sistema deve:

- Debitar o valor da conta de origem  
- Creditar o valor da conta de destino  
- Registrar data/hora e valor da operação  

### Em caso de erro:

- Exibir uma mensagem clara  
- Não alterar nenhum saldo das contas  
