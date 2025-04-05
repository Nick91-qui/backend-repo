# backend-repo
Site para inscrição de alunos e tutores



📦 Deploy
Conecte o repositório ao Render
Configure as variáveis de ambiente no Render:
MONGODB_URI
FRONTEND_URL
PORT
🛠️ Estrutura do Projeto

backend/
├── config/
│   └── db.js
├── routes/
│   └── index.js
├── models/
├── server.js
└── package.json
📝 API Endpoints
POST /api/verificar-aluno

Verifica se o aluno está cadastrado
Body: { turma: string, nome: string }
POST /api/preferencias

Salva as preferências do aluno
Body: { turma: string, nome: string, preferencias: array }
GET /api/admin/estatisticas

Retorna estatísticas do sistema
Requer autenticação
⚙️ Otimizações
Cache implementado para consultas frequentes
Rate limiting por IP
Compressão de dados
Tratamento de concorrência
Logs de monitoramento
