# COMO CRIAR UM SERVIDOR HTTP COM NODEJS E EXPRESS

### Primeiro, certifique-se de que o Node.js está instalado no seu computador. Acesse nodejs.org e baixe a versão LTS mais recente. Após a instalação, abra o terminal e digite:
```
node -v
```

### Crie uma pasta para o projeto e navegue até ela no terminal. Depois, execute o comando:
```
npm init -y
```

### Agora, instale o Express com o seguinte comando:
```
npm install express
```

### Dentro da pasta do projeto, crie um arquivo chamado index.js. Adicione o seguinte código:
```
const express = require('express');
const app = express();

app.get('/', (req, res) => {
    res.send('Servidor rodando com Express!');
});

app.listen(3000, () => {
    console.log('Servidor rodando em http://localhost:3000');
});
```

### Volte ao terminal e execute o comando:
```
node index.js
```

### Abra o navegador e acesse http://localhost:3000 Pronto! Você criou seu primeiro servidor HTTP com Node.js e Express.
