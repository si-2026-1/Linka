# HU-[ID]: [Título Conciso e Direto da Funcionalidade]

**Ator Principal:** [Ex: Gerente Comercial, Cliente, Administrador]  
**Módulo do Sistema:** [Ex: Módulo de Vendas / Sub-sistema Gastronômico]

---

### 1. Descrição Narrativa
> **Como** [Papel/Ator do sistema que se beneficia da funcionalidade],  
> **Gostaria de** [Ação ou capacidade que deseja executar no sistema],  
> **Para** [O valor de negócio gerado ou o problema que resolve].

---

### 2. Checklist de Componentes da Interface (UI/UX)
*O que a tela ou o fluxo precisa conter visualmente para o usuário interagir:*
- [ ] Formulário ou campos de entrada para: `[Listar dados de entrada]`
- [ ] Questionário/Perguntas guia para inserção assistida
- [ ] Exibição dinâmica de dados em tempo real (Gráfico, Tabela ou Dashboard)
- [ ] Botões de ação explícitos (`Salvar`, `Cancelar`, `Excluir`, `Efetuar Pagamento`)
- [ ] Indicador visual de progresso ou estado (`Pendente`, `Concluído`, `Erro`)

---

### 3. Critérios de Aceitação (Regras de Negócio e Validações)
*O comportamento esperado do sistema e suas restrições lógicas:*

#### Fluxo Principal (Sucesso):
* **Cenário 1: Inserção/Execução Válida**
  * **Dado** que o usuário preencheu todos os campos obrigatórios corretamente,
  * **Quando** ele acionar a ação de confirmação,
  * **Então** o sistema deve persistir a informação e gerar o número identificador único sequencial automaticamente.

#### Fluxo de Exceção (Validações e Tratamento de Erros):
* **Cenário 2: Bloqueio por Limite Quantitativo**
  * *Exemplo de Regra:* Emitir erro impeditivo caso a ação viole uma restrição de capacidade (ex: atribuir tarefa a quem já atingiu o limite máximo de X).
* **Cenário 3: Validação Baseada em Estado Anterior**
  * *Exemplo de Regra:* Bloquear edições que tentem rebaixar valores ou metas abaixo do que já foi consolidado/atingido historicamente.
* **Cenário 4: Limitação Percentual/Regra de Teto**
  * *Exemplo de Regra:* Bloquear reajustes ou alterações que superem a margem de X% estipulada pelas diretrizes organizacionais.
* **Cenário 5: Consistência de Saldos e Valores**
  * *Exemplo de Regra:* Impedir registros de transações parciais que superem o valor total pendente da entidade (ex: pagamento maior que o saldo devedor).

---

### 4. Impacto Estrutural e Arquitetura de Dados
*Mapeamento lógico de quais dados e estados são manipulados por esta HU:*

* **Coleções/Entidades Afetadas:** `[Ex: orders, tables, users]`
* **Atributos Modificados/Atualizados:**
  * `status`: transiciona de `[Estado A]` para `[Estado B]`.
  * `balance` / `totalSpent`: cálculos automáticos acionados de subtração ou incremento.
