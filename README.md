# Bellita Cosmetics — protótipo com carrinho e checkout Mercado Pago

## Abrir no VS Code
1. Extraia o ZIP e abra esta pasta no VS Code.
2. Instale Node.js 18+.
3. **Não** use Live Server para testar pagamentos. O checkout precisa do servidor.
4. No terminal do VS Code (PowerShell), defina um **novo token** apenas na sessão atual: `$env:MERCADOPAGO_ACCESS_TOKEN="SEU_NOVO_TOKEN"`.
5. Execute `npm start` e abra http://localhost:3000.
6. Clique em **Adicionar ao carrinho** e depois **Ir para o checkout seguro**.

## Atenção à segurança e ao ambiente
- O Access Token e as senhas enviados no chat **não** estão presentes no código. Revogue o token exposto e gere outro no Mercado Pago.
- Para testes, use credenciais e contas de **teste/sandbox** conforme as instruções do Mercado Pago; nunca execute cobranças reais por engano.
- O Mercado Pago pode exigir uma URL pública HTTPS para configurar os `back_urls` e notificações. Ajuste `PUBLIC_BASE_URL` no servidor quando houver domínio público.
- A página de confirmação consulta o status do pagamento via API. Para processar pedidos reais, falta implementar banco de dados, cálculo de frete, dados do comprador, controle de estoque, webhooks com validação de assinatura, reconciliação e política de privacidade.
- Os preços são exemplos do site consultado anteriormente; confirme antes de usar em produção.
- O protótipo não substitui automaticamente a Loja Integrada. O carrinho e checkout aqui são separados do carrinho oficial.
- A logo original foi apenas ampliada e recebeu leve nitidez. Não foi redesenhada.


## Correções desta versão
- Logo original recortada, ampliada e com fundo transparente.
- Imagens de produtos exibidas em área branca uniforme para eliminar bordas brancas visíveis sem adulterar embalagens.
- Botão de cada produto alinhado ao seu próprio card.
- Checkout informa quando o site é aberto no Live Server (porta 5500). Use `http://localhost:3000`.
- Nunca publique credenciais do Mercado Pago no HTML. Use token novo em variável de ambiente no servidor.


## Atualização de conteúdo
- Depoimentos: `depoimentos.html`
- Histórias de Superação: `superacao.html`
- Cadastro de revendedora: link direto na navegação.
- Logo: `assets/logo-bellita.png` (imagem enviada pelo cliente).
- A menção ao selo UFG é uma alegação fornecida pelo solicitante e requer comprovação documental antes de publicação comercial.
- Abra em http://localhost:3000 (não Live Server 5500) para checkout.


## Atualização do menu
Produtos contém Rotina Luminus; Nossa História contém Depoimentos e Histórias de Superação. Minha Conta direciona à loja oficial. O contador do carrinho foi ocultado visualmente, mas continua acessível a leitores de tela. A marca UFG é carregada da página oficial da universidade, exigindo internet. A referência ao selo não comprova certificação ou endosso; confirme a autorização e documentação antes de publicar.


## Identidade visual
Imagem transparente da seção Tecnologia e pesquisa: `assets/ufg-tecnologia-pesquisa.png`. Favicon Bellita: `assets/favicon-bellita.png` e `.ico`.
A arte da UFG fornecida pelo usuário não deve ser tratada como certificação institucional sem documentação.
