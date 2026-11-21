# aplicativo ai-studio-firebase

Aplicativo web integrado com **Firebase** (Hosting e Analytics) e **Google AI Studio**, estruturado com arquitetura limpa e boas práticas de segurança por meio de variáveis de ambiente (`VITE_FIREBASE_*`).

## Destaques do projeto

* **Firebase (Hosting & Analytics):** base preparada para inicialização do aplicativo, hospedagem web e acompanhamento de métricas.
* **Google AI Studio:** estrutura pensada para evoluir funcionalidades e integrações com inteligência artificial.
* **Segurança de credenciais:** separação entre o arquivo de exemplo (`.env.example`) e as credenciais locais (`.env`), ignoradas pelo Git via `.gitignore`.

## Estrutura do repositório

```text
ai-studio-firebase-app/
├── src/
├── .env.example
├── .gitignore
├── index.html
└── README.md
