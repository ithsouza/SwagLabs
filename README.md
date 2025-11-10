# 🧪 SwagLabs — QA Challenge (Entrega Resumida)

Documentação resumida para o desafio de QA Manual da **DIO** utilizando o contexto da loja virtual **SwagLabs Shopping**.

---

## 📘 Contexto do Projeto
O **SwagLabs Shopping** é uma loja virtual que permite ao usuário realizar login, navegar pelos produtos, adicionar itens ao carrinho e finalizar uma compra.

Esta entrega resume os principais artefatos de QA, seguindo boas práticas ágeis e técnicas de documentação de testes manuais.

---

## 🧭 Workflow e Ciclo de Vida do Bug
**Workflow:**

**Ciclo de Vida do Bug:**

 
---

## 🧩 User Stories

### US01 — Autenticação do Usuário
**Como** um comprador registrado,  
**Quero** fazer login com email e senha,  
**Para** acessar minha conta e finalizar pedidos.

**Critérios de aceite:**
- Email e senha válidos redirecionam para a página de produtos.  
- Mensagem de erro exibida para credenciais inválidas.

---

### US02 — Finalizar Compra
**Como** um comprador,  
**Quero** adicionar produto ao carrinho e finalizar compra,  
**Para** concluir o pedido e receber confirmação.

**Critérios de aceite:**
- Carrinho exibe produto, quantidade e total.  
- Checkout solicita endereço e forma de pagamento.  
- Exibe número de pedido após conclusão.

---

## 🧠 Mind-map (US02 — Checkout)
Checkout
├─ Carrinho
│ ├─ Listagem produtos
│ ├─ Quantidade (editar)
│ └─ Total (cálculo)
├─ Endereço
│ ├─ CEP
│ ├─ Rua
│ └─ Número
├─ Pagamento
│ ├─ Cartão de Crédito
│ ├─ Boleto
│ └─ Validação de dados
└─ Confirmação
├─ Resumo do pedido
└─ Número de pedido




---

## 🧾 Casos de Teste

### Caso A — Step-by-step (Login válido)
**Pré-condição:** Usuário cadastrado.  
**Passos:**  
1. Acessar página de login  
2. Inserir credenciais válidas  
3. Clicar em “Entrar”  
**Resultado esperado:**  
Usuário acessa a página de produtos e vê saudação no cabeçalho.

---

### Caso B — BDD (Checkout com cartão válido)
**Cenário:** Finalizar compra com sucesso  
**Dado que** o usuário está logado e possui produto no carrinho,  
**Quando** ele preenche dados de pagamento válidos e confirma,  
**Então** o sistema cria um pedido e exibe o número de confirmação.

---

## 📂 Estrutura do Repositório
swaglabs-qa/
├─ docs/
│ ├─ workflow_bug_lifecycle.pdf
│ ├─ user_stories.pdf
│ ├─ mindmap_checkout.pdf
│ └─ test_cases.pdf
├─ SwagLabs_QA_Entrega_Resumida.pdf
└─ README.md



---

## 🚀 Como Utilizar
1. Abra os PDFs da pasta `docs/` para visualizar os artefatos.  
2. Execute os casos de teste manualmente em ambiente de QA.  
3. Registre os resultados, evidências e bugs conforme o fluxo definido.

---

## ✍️ Autor
**Thiago Francisco**  
Desafio de QA Manual — DIO 🌐 



