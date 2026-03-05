# Casos de Uso – Sistema de E-commerce

---

## Caso de Uso 1: Realizar Pedido

**Ator:** Cliente  
**Objetivo:** Comprar um ou mais produtos através do sistema

### Pré-condições
- Cliente estar logado
- Produtos estarem disponíveis em estoque

### Pós-condições
- Pedido registrado no sistema
- Estoque atualizado

### Fluxo Principal
1) Cliente acessa o catálogo de produtos.
2) Cliente seleciona um produto e adiciona ao carrinho.
3) Sistema exibe o carrinho com os itens selecionados.
4) Cliente informa endereço de entrega.
5) Cliente escolhe forma de pagamento.
6) Cliente confirma o pedido.
7) Sistema gera número de pedido e exibe confirmação.
8) Sistema envia e-mail de confirmação.

### Fluxos Alternativos
**A1 - Carrinho vazio:**
  1) Cliente tenta finalizar pedido sem itens.
  2) Sistema exibe mensagem: "Adicione itens ao carrinho primeiro".
  3) Redireciona para o catálogo.

**A2 - Produto sem estoque:**
  1) Ao adicionar ao carrinho, sistema verifica estoque insuficiente.
  2) Sistema informa: "Produto sem estoque disponível".
  3) Permite que cliente cadastre alerta de disponibilidade.

### Regras de Negócio
- RN01: Pedido mínimo de R$ 10,00
- RN02: Estoque só é baixado após confirmação do pagamento

### Requisitos Relacionados
- RF02 Gerenciar carrinho
- RF03 Processar pagamento
- RNF02 Disponibilidade 99,5%

---

## Caso de Uso 2: Cancelar Pedido

**Ator:** Cliente  
**Objetivo:** Cancelar um pedido que ainda não foi enviado

### Pré-condições
- Pedido estar com status "Aguardando pagamento" ou "Pagamento confirmado"
- Pedido não ter sido enviado

### Pós-condições
- Pedido cancelado
- Estoque dos produtos é restituído (se pagamento já confirmado)

### Fluxo Principal
1) Cliente acessa "Meus Pedidos".
2) Cliente seleciona o pedido que deseja cancelar.
3) Sistema exibe opção "Cancelar Pedido".
4) Cliente confirma o cancelamento.
5) Sistema altera status para "Cancelado".
6) Sistema envia e-mail de confirmação de cancelamento.

### Fluxos Alternativos
**A1 - Pedido já enviado:**
  1) Cliente tenta cancelar pedido com status "Enviado".
  2) Sistema informa: "Pedido já foi enviado, não é possível cancelar".
  3) Oferece opção de solicitar troca ou devolução.

### Regras de Negócio
- RN03: Cancelamento permitido apenas em até 7 dias após a compra (CDC)
- RN04: Estoque é restituído automaticamente

### Requisitos Relacionados
- RF04 Gerenciar pedidos
- RNF03 Segurança nos dados do cliente

---

## Caso de Uso 3: Avaliar Produto

**Ator:** Cliente  
**Objetivo:** Atribuir nota e comentário a um produto comprado

### Pré-condições
- Cliente ter comprado o produto
- Pedido estar com status "Entregue"

### Pós-condições
- Avaliação registrada no sistema
- Produto tem média de avaliações atualizada

### Fluxo Principal
1) Cliente acessa "Meus Pedidos".
2) Cliente seleciona um pedido entregue.
3) Cliente clica em "Avaliar Produto" para um dos itens.
4) Sistema exibe formulário com nota (1 a 5) e campo de comentário.
5) Cliente preenche e envia avaliação.
6) Sistema registra avaliação e atualiza média do produto.
7) Sistema exibe mensagem: "Avaliação enviada com sucesso".

### Fluxos Alternativos
**A1 - Avaliação editada:**
  1) Cliente acessa avaliação já existente.
  2) Sistema permite editar nota e comentário.
  3) Cliente confirma alterações.
  4) Sistema atualiza registro.

### Regras de Negócio
- RN05: Cliente só pode avaliar produtos comprados e entregues
- RN06: Apenas uma avaliação por produto por cliente

### Requisitos Relacionados
- RF05 Gerenciar avaliações
- RNF04 Resposta em até 3s
