# Backlog do Sistema - E-commerce

---

## Épico 1 — Catálogo e Produtos
**Descrição:** Gerenciamento e exibição do catálogo de produtos.

### User Stories
- **US01 — Visualizar catálogo de produtos**  
  *Como cliente, quero ver todos os produtos disponíveis para escolher o que comprar.*

- **US02 — Buscar produtos**  
  *Como cliente, quero buscar produtos por nome ou categoria para encontrar rapidamente o que procuro.*

- **US03 — Visualizar detalhes do produto**  
  *Como cliente, quero ver informações detalhadas do produto (descrição, fotos, preço) para decidir se compro.*

- **US04 — Filtrar produtos**  
  *Como cliente, quero filtrar produtos por preço, categoria ou avaliação para refinar minha busca.*

- **US05 — Ver avaliações de produtos**  
  *Como cliente, quero ler avaliações de outros clientes para saber a opinião sobre o produto.*

---

## Épico 2 — Carrinho e Checkout
**Descrição:** Gerenciamento do carrinho de compras e processo de finalização do pedido.

### User Stories
- **US10 — Adicionar produto ao carrinho**  
  *Como cliente, quero adicionar produtos ao carrinho de compras para reunir os itens que desejo comprar.*

- **US11 — Visualizar carrinho**  
  *Como cliente, quero ver os itens no meu carrinho para revisar antes de comprar.*

- **US12 — Remover item do carrinho**  
  *Como cliente, quero remover itens do carrinho caso mude de ideia.*

- **US13 — Alterar quantidade de itens**  
  *Como cliente, quero aumentar ou diminuir a quantidade de produtos no carrinho para comprar múltiplas unidades.*

- **US14 — Calcular frete**  
  *Como cliente, quero calcular o frete informando meu CEP para saber o custo de entrega.*

- **US15 — Aplicar cupom de desconto**  
  *Como cliente, quero inserir um cupom de desconto para pagar menos.*

---

## Épico 3 — Pedidos e Pagamento
**Descrição:** Processamento de pedidos, integração com meios de pagamento e confirmação de compras.

### User Stories
- **US20 — Informar endereço de entrega**  
  *Como cliente, quero informar o endereço onde o pedido será entregue para receber minha compra.*

- **US21 — Escolher forma de pagamento**  
  *Como cliente, quero escolher entre cartão, pix ou boleto para pagar de forma conveniente.*

- **US22 — Confirmar pedido**  
  *Como cliente, quero revisar todos os dados e confirmar a compra para finalizar o pedido.*

- **US23 — Receber confirmação do pedido**  
  *Como cliente, quero receber um e-mail de confirmação para ter o comprovante da compra.*

- **US24 — Pagar com cartão de crédito**  
  *Como cliente, quero parcelar minha compra no cartão para dividir o valor.*

- **US25 — Gerar boleto bancário**  
  *Como cliente, quero gerar um boleto para pagar à vista.*

---

## Épico 4 — Gerenciamento de Pedidos
**Descrição:** Acompanhamento e gestão dos pedidos realizados pelos clientes.

### User Stories
- **US30 — Acompanhar pedido**  
  *Como cliente, quero acompanhar o status do meu pedido para saber quando será entregue.*

- **US31 — Visualizar histórico de pedidos**  
  *Como cliente, quero ver todos os pedidos que já fiz para consultar compras anteriores.*

- **US32 — Cancelar pedido**  
  *Como cliente, quero cancelar um pedido que ainda não foi enviado para não receber produtos que não quero mais.*

- **US33 — Solicitar troca/devolução**  
  *Como cliente, quero solicitar troca ou devolução de um produto para resolver problemas com a compra.*

- **US34 — Ver detalhes do pedido**  
  *Como cliente, quero ver informações completas do pedido (itens, valor, endereço) para conferência.*

---

## Épico 5 — Avaliações e Feedback
**Descrição:** Sistema de avaliações de produtos e feedback dos clientes.

### User Stories
- **US40 — Avaliar produto comprado**  
  *Como cliente, quero dar uma nota e comentário para produtos que comprei para ajudar outros clientes.*

- **US41 — Editar avaliação**  
  *Como cliente, quero editar minha avaliação caso queira complementar ou corrigir informações.*

- **US42 — Responder avaliações**  
  *Como vendedor, quero responder avaliações dos clientes para esclarecer dúvidas ou agradecer.*

- **US43 — Reportar avaliação inadequada**  
  *Como cliente, quero denunciar avaliações com conteúdo impróprio para manter a comunidade saudável.*

- **US44 — Ver média de avaliações**  
  *Como cliente, quero ver a nota média dos produtos para saber a reputação deles.*

---

## Épico 6 — Administração e Gestão
**Descrição:** Funcionalidades administrativas para gerenciar produtos, pedidos e usuários.

### User Stories
- **US50 — Cadastrar produto**  
  *Como administrador, quero cadastrar novos produtos para disponibilizá-los na loja.*

- **US51 — Editar produto**  
  *Como administrador, quero editar informações de produtos para mantê-las atualizadas.*

- **US52 — Remover produto**  
  *Como administrador, quero remover produtos que não estão mais disponíveis.*

- **US53 — Gerenciar estoque**  
  *Como administrador, quero controlar o estoque dos produtos para evitar vendas sem estoque.*

- **US54 — Visualizar pedidos recebidos**  
  *Como administrador, quero ver todos os pedidos realizados para gerenciar entregas.*

- **US55 — Atualizar status do pedido**  
  *Como administrador, quero atualizar o status do pedido (enviado, entregue) para manter o cliente informado.*

- **US56 — Gerenciar usuários**  
  *Como administrador, quero visualizar e gerenciar contas de usuários para administrar acessos.*

---

## Relação com Casos de Uso

| Caso de Uso | Épico Relacionado | Stories Correspondentes |
|-------------|-------------------|-------------------------|
| Realizar Pedido | Épico 2 e 3 | US10, US11, US20, US21, US22, US23 |
| Cancelar Pedido | Épico 4 | US32 |
| Avaliar Produto | Épico 5 | US40, US41, US44 |

## MVP (Mínimo Produto Viável)

Stories essenciais para o fluxo principal do Caso de Uso "Realizar Pedido":

- US01 — Visualizar catálogo
- US10 — Adicionar ao carrinho
- US11 — Visualizar carrinho
- US20 — Informar endereço
- US21 — Escolher pagamento
- US22 — Confirmar pedido
- US23 — Receber confirmação
