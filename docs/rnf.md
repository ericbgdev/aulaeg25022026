## 3. Regras de Negócio (RN)

### RN01 — Maioridade
Para criar uma conta, o usuário deve ter mais de 18 anos.

### RN02 — Bloqueio por inatividade
Usuários inativos por mais de 90 dias devem ser marcados como inativos.

### RN03 — Limite de tentativas de login
Após 5 tentativas inválidas, a conta deve ser temporariamente bloqueada.

### RN03 — Limite de tentativas de login
Após 5 tentativas de login com senha inválida em um período de 15 minutos, a conta deve ser temporariamente bloqueada por 30 minutos.

### RN04 — Complexidade de senha
A senha do usuário deve conter pelo menos 8 caracteres, incluindo letras maiúsculas, minúsculas, números e caracteres especiais.

### RN05 — Exclusão de conta
A exclusão da conta só pode ser solicitada pelo próprio usuário, através do fluxo de "Encerrar conta", e a remoção definitiva dos dados deve ocorrer após 30 dias (período de arrependimento).

### RN06 — Verificação de e-mail
O usuário só poderá acessar totalmente a plataforma após confirmar o endereço de e-mail através de um link enviado no ato do cadastro.

### RN07 — Troca de e-mail
Qualquer solicitação de alteração de e-mail deve ser confirmada através de um link enviado para o novo endereço, invalidando o e-mail anterior imediatamente após a confirmação.

### RN08 — Perfil público
Usuários podem optar por tornar seu perfil público ou privado. Perfis privados não aparecem em buscas para usuários não autenticados.
