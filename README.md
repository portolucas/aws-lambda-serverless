
# Serverless

Olá! Meu nome é Lucas, sou professor da pós-graduação da **PUC Minas**. Este é um projeto para os alunos da pós-graduação.

# Start

Vamos começar pela abordagem Serverless.

Vamos utilizar o Serverless Framework. Crie uma conta clicando [aqui](https://app.serverless.com/).
Para seguir com o tutorial, você deve ter uma conta na AWS. Entre ou crie uma conta clicando [aqui](https://portal.aws.amazon.com/billing/signup?nc2=h_ct&src=header_signup&redirect_url=https://aws.amazon.com/registration-confirmation&language=pt_br#/start/email).

Uma vez que você criou uma conta na AWS, precisamos vincular essa conta à conta do Serverless Framework.

Para isso, entre na plataforma do Serverless Framework, clique em **org** -> **provider** -> **add**. Nomeie seu provider e clique em **Connect AWS Provider**. Por fim, vá à aba **apps** -> **create app** -> e nomeie o seu app. Selecione o template **Node HTTP API**. Quando você terminar, vai aparecer um modal com um código. Copie esse código e cole no seu terminal.

O seu código deve se parecer com esse:

```
npm i -g serverless && serverless \
--org=lucasporto \
--app=aws-hello-world \
--name=aws-hello-world \
--template=aws-node-http-api
```

## Files and folders

Agora podemos acessar o diretorio onde você executou o código acima e ver os arquivos que foram baixados:
- Temos uma pasta **.serverless** com as configurações que o próprio framework criou para nós;
- Arquivo **index.js** com o nosso primeiro handler.

Como nós já adicionamos a AWS como provider no dashboard do Serverless Framework, podemos fazer o deploy que o próprio framework vai detectar as keys necessárias e criar os serviços necessários para subir a nossa aplicação serverless.

Execute o seguinte comando:
```
sls deploy
```

Aguarde a execução e pronto, temos uma aplicação rodando. No seu console aparecerá a url da sua api para podermos acessar os seus recursos.

Acesse a AWS Lambda, identifique a sua lambda e teste o seu código no console.

  

