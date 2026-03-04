## 2. Requisitos Não Funcionais (RNF)

### RNF01 — Tempo de resposta
O sistema deve carregar telas principais em até **2 segundos**.

### RNF02 — Segurança
As senhas devem ser armazenadas usando hash seguro (ex.: bcrypt).

### RNF03 — Compatibilidade
O sistema deve funcionar nos navegadores Chrome, Edge e Firefox.
### RNF04 — Disponibilidade
O sistema deve estar disponível (uptime) pelo menos 99,5% do tempo mensal.

### RNF05 — Responsividade
A interface do usuário deve ser adaptável para dispositivos móveis (smartphones e tablets) e desktops.

### RNF06 — Criptografia de Dados
Todos os dados transmitidos entre o cliente e o servidor devem ser protegidos via protocolo HTTPS/TLS.

### RNF07 — Escalabilidade
O sistema deve ser capaz de suportar até 1.000 usuários simultâneos sem perda de desempenho.

### RNF08 — Manutenibilidade
O código-fonte deve ser documentado e seguir padrões de arquitetura (como MVC ou Clean Architecture) para facilitar futuras atualizações.
