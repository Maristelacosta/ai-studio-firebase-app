# AI Studio Firebase App

Aplicação web integrada ao Firebase Hosting e Analytics, preparada para evoluir com integrações do Google AI Studio.

## Tecnologias

- HTML e JavaScript
- Vite
- Firebase Hosting
- Firebase Analytics
- Google AI Studio

## Pré-requisitos

- Node.js 20 ou superior
- npm
- Conta no Firebase
- Firebase CLI:

```bash
npm install -g firebase-tools
```

## Instalação

```bash
git clone https://github.com/Maristelacosta/ai-studio-firebase-app.git
cd ai-studio-firebase-app
npm install
```

## Configuração do Firebase

1. Crie um projeto no [Firebase Console](https://console.firebase.google.com/).
2. Ative o Firebase Hosting e o Analytics.
3. Crie o arquivo `.env` a partir do modelo:

```bash
cp .env.example .env
```

4. Preencha as variáveis no arquivo `.env`:

```env
VITE_FIREBASE_API_KEY=sua-api-key
VITE_FIREBASE_AUTH_DOMAIN=seu-projeto.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=seu-projeto
VITE_FIREBASE_STORAGE_BUCKET=seu-projeto.appspot.com
VITE_FIREBASE_MESSAGING_SENDER_ID=seu-sender-id
VITE_FIREBASE_APP_ID=seu-app-id
VITE_FIREBASE_MEASUREMENT_ID=seu-measurement-id
```

Nunca publique um arquivo `.env` com credenciais reais no Git.

## Executar localmente

```bash
npm run dev
```

A aplicação ficará disponível em `http://localhost:5173`.

## Scripts

```bash
npm run dev      # Inicia o servidor de desenvolvimento
npm run build    # Cria a versão de produção
npm run preview  # Visualiza a versão de produção
```

## Deploy

```bash
firebase login
firebase use --add
npm run build
firebase deploy
```

## Estrutura do projeto

```text
.
├── src/
│   └── firebase.js
├── .env.example
├── .gitignore
├── index.html
├── package.json
├── firebase.json
└── README.md
```

## Boas práticas de segurança

- Mantenha `.env` no `.gitignore`.
- Não registre no repositório credenciais administrativas ou chaves privadas.
- Restrinja as regras de segurança do Firebase.
- Use variáveis de ambiente para configurações específicas de cada ambiente.
- Revise a documentação do Firebase antes de publicar dados sensíveis.

## Próximos passos

- Adicionar componentes de interface.
- Integrar funcionalidades do Google AI Studio.
- Implementar autenticação.
- Configurar testes automatizados.
- Adicionar monitoramento de erros.
- Configurar ambientes de desenvolvimento e produção.

## Licença

Defina aqui a licença do projeto, por exemplo MIT.
