## Olá, parceiro de software e revenda TEF!
🔊 **Descubra tudo sobre TEF, incluindo suas funcionalidades, etapas de uso e pontos técnicos.**
![image.png](/knowledge/imagens/6acb9a3ca0d0844140de3a52) 
## 🔌 O que é TEF?
O TEF (*Transferência Eletrônica de Fundos*) é uma solução multiadquirente (explicaremos à seguir) que possibilita vendas no crédito, débito, voucher e PIX, garantindo muito mais agilidade e segurança para o seu negócio.<br/>

## 🤔 Como funciona o TEF?

Por meio do TEF, a comunicação entre o PDV (ponto de venda/sistema de vendas), integrador TEF e autorizadores (adquirentes/bancos) ocorre de forma ordenada.<br/>

O uso de autorizadores/adquirentes é possível devido, também, ao uso do PINPad, ou comumente chamada, "a maquininha". Tratamos mais sobre ela no tópico "O que é e como utilizar PINPad?"  (https://elgin.hubdns.com.br/elgin-tef-hub/o-que-e-e-como-utilizar-pinpad).

### 💬 As transações podem ser realizadas por mais de uma adquirente?

👉 Isso mesmo! Multiadquirente (*mais de uma adquirente*)!<br/>
Por meio do TEF é possível que transações, por exemplo, via débito sejam roteadas por uma adquirente e transações crédito sejam roteadas por outra adquirente. Podendo escolher a melhor condição comercial para o seu negócio.

Com isso, não é necessário possuir uma maquininha de cada adquirente. 

> Com "adquirente" me refiro à Rede, Cielo, Stone, Getnet, Vero e afins.

### 💬 Como eu faço essa configuração de Multiadquirente?
Primeiramente o cliente/lojista deve realizar o contato com as adquirente desejadas.

✏️ **Por exemplo:** 

Sou um lojista e desejo utilizar a adquirente "X" em transações débito e adquirente "Y" em transações crédito.

> "X": Uma adquirente 
 "Y": Outra adquirente

🔹**Passo 1:** Eu, lojista, devo entrar em contato com o time das adquirentes "X" e "Y", informar que desejo utilizar TEF com eles, e assim solicitar as credenciais TEF (Número lógico e Código do Estabelecimento comercial).

🔹**Passo 2:** Em seguida, eu, lojista, devo entrar em contato com o time do sistema de vendas/revenda do sistema de vendas e informar que desejo utilizar TEF, com a adquirente "X" via débito e "Y" via crédito.

🔹**Passo 3:** O time do sistema de vendas/revenda do sistema de vendas me encaminhará esta planilha: [❌Anexar aqui a planilha de roteamento❌]

🔹**Passo 3:** Eu, lojista, preencherei a planilha e encaminharei ao time do sistema de vendas.

🔹**Passo 4:** O time do sistema de vendas/revenda do sistema de vendas, anexará esta planilha no pedido TEF (via https://tefelgin2.com.br/). Manual: [❌Colocar link com  o manual❌] 

🔹**Passo 5:** O time da Elgin realizará o procedimento de roteamento de multibandeiras no servidor.

> Com "multibandeiras" me refiro à Master, Visa, Elo, Cabal e afins. Bandeiras de cartões.

O prazo médio (SLA) de realização por parte da Elgin é de ❌ dias.

### 💬 Entendi. Então cada um tem uma responsabilidade/ação à realizar, isso?

👉 Isso mesmo!

Confira o fluxo ocorrido em transações TEF via cartão:

![FluxoTEF.png](/knowledge/imagens/6accde70a0d0844140de3a56)

1️⃣ **Operador:** O valor é informado e o cliente apresenta o cartão (débito, crédito ou voucher) na maquininha (PINPad). 

2️⃣ **Sistema de vendas (PDV):** O sistema de vendas (PDV) captura, valida e formata os dados da transação. Em seguida, encaminha para a TEF House.

3️⃣**TEF House (Motor TEF):** A TEF House (servidor) recebe as informações e repassa para a adquirente previamente configurada.

4️⃣**Adquirente:** A adquirente recebe, processa a transação e encaminha para a bandeira.

5️⃣**Bandeira:** A bandeira analisa e roteia a transação para o banco emissor.

6️⃣**Banco Emissor:** O banco emissor autoriza ou não a transação.

7️⃣**Banco Emissor:** Retorna o resultado para a bandeira.

8️⃣**Bandeira:** Recebe o resultado da operação e encaminha para a adquirente.

9️⃣**Adquirente:** A adquirente recebe o resultado da operação, organiza os dados e forma o comprovante de venda TEF.

🔟**TEF House (Motor TEF):** Com o comprovante e  dados  recebidos da adquirente, os organiza para o PDV.

1️⃣1️⃣**Sistema de vendas (PDV):** Recebe os dados TEF, apresenta a mensagem resultado ao operador e, em caso de sucesso, imprime o comprovante TEF.

1️⃣2️⃣**Operador:** Lê a mensagem retornada e informa o consumidor.

Tudo ocorre em poucos segundos e com comunicação criptografada em cada etapa, garantindo a segurança dos dados do seu cliente.

## 🧭 Conhecendo as etapas
### 🖥️ Sistema de vendas

É também conhecido como ponto de venda (PDV), ERP ou frente de caixa.

Usado para cadastrar produtos, controlar estoque e vendas, assim como realizar o fechamento do caixa e efetuar emissão de notas fiscais. 

É nessa tela que o operador registra os itens vendidos e escolhe a forma de pagamento.<br/>
### 🌉 TEF House (Motor TEF)

A TEF é quem recebe a venda que iniciou no sistema de vendas (PDV/ERP/frente de caixa) e encaminha para a(s) adquirente(s).

Funcionando como uma ponte de comunicação que direciona cada transação para a adquirente escolhida e é o que o torna TEF multiadquirente.<br/>

### 📡 Adquirente

É quem gera as credenciais (Número Lógico/Número do Estabelecimento Comercial) e processa as transações.<br/>

### 💳 Bandeira

As mais conhecidas são MasterCard, Visa, Elo, American Express, Banrisul e entre outras.

Ao entrar em contato com a adquirente "X", eles configurarão o Mastercard, Visa, Elo e American Express diretamente no servidor deles. 

A depender da bandeira do cartão, como 'VR', a **modalidade** será **VAN** (liquidação externa, como vouchers e bandeiras regionais). Nestes casos será necessário que o lojista entre em contato com o time da bandeira e também com a adquirente por ele utilizada, e assim, solicitar a habilitação com os dois.

> **Todas as demais são bandeiras VAN**, com liquidação feita diretamente pela própria bandeira. Por isso, mantenha seu cadastro regular junto às bandeiras VAN nas quais possui afiliação.

### 💬 Entendi. Então o TEF Hub Elgin é uma TEF House?

Não, o TEF Hub Elgin trabalha com as TEF Houses. Ele é exatamente um *Hub* (centro/ponto de conexão) com várias TEF Houses.

Hoje o TEF Hub Elgin possui integrado os motores (TEF Houses):

-> Fiserv (SITEF);
-> Destaxa (VBI);
-> Conexão Tech (Scope);
-> Auttar (CTF).

Ou seja, utilizando o TEF Hub Elgin não é necessário limitar-se ás opções de uma só TEF House.  [❌ Essa parte aqui pode melhorar. Ser mais comercial ❌] 

## ❓ Suporte e Dúvidas
Em caso de dúvidas, entre em contato com nosso suporte via WhatsApp:

📱 [**Clique aqui para falar com o atendimento**](https://api.whatsapp.com/send/?phone=%2B5511998519559&text&type=phone_number&app_absent=0)
