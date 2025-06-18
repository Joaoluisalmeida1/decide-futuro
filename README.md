# Decide.Futuro – Plataforma de Orientação Pós-Secundária

## 🚀 Visão Geral

Decide.Futuro é uma plataforma inovadora para ajudar alunos do ensino secundário a tomar decisões informadas sobre o seu futuro académico e profissional. A aplicação oferece testes de perfil, recomendações de cursos, simulador de candidatura DGES, marketplace de mentores universitários/profissionais, dashboards para escolas e muito mais.

---

## 🧑‍💻 Tech Stack Sugerido

- **Frontend:** React (Vite ou Create React App), TypeScript, TailwindCSS ou Material UI
- **Backend:** Node.js (Express ou NestJS), TypeScript
- **Base de Dados:** PostgreSQL (alternativa: MongoDB)
- **Autenticação:** Auth0, Firebase Auth ou JWT customizado
- **Videochamadas/Chat:** Twilio, Daily.co, Jitsi ou WebRTC custom
- **Pagamentos:** Stripe Connect
- **Infraestrutura:** Docker, GitHub Actions (CI/CD), Vercel/Netlify (frontend), Heroku/Render/AWS (backend)
- **Scraping/Estatísticas:** Python scripts (BeautifulSoup, Scrapy) ou APIs públicas (INE, IEFP, LinkedIn)
- **PDF Reports:** Puppeteer ou jsPDF

---

## 📦 Estrutura Inicial do Projeto

```
decide-futuro/
│
├── frontend/         # React app
│   ├── public/
│   └── src/
│       ├── components/
│       ├── pages/
│       ├── hooks/
│       ├── services/
│       └── App.tsx
│
├── backend/          # Node.js API
│   ├── src/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── services/
│   │   └── app.ts
│   └── prisma/       # (caso use Prisma ORM)
│
├── scripts/          # Scraping, ETL, etc.
│
├── docs/             # Documentação adicional
│
├── docker-compose.yml
├── README.md
└── package.json
```

---

## 🧩 Funcionalidades Principais

### 1. Teste de Perfil + Recomendação de Cursos
- Formulário dinâmico (React) para recolher interesses, notas, localização.
- Algoritmo de matching (backend) para sugerir cursos.
- Exibição de médias de entrada, saídas profissionais, salários, empregabilidade.

### 2. Simulador de Candidatura DGES
- Simulação de candidatura com base nas notas e preferências.
- Algoritmo para sugerir ordem ótima de cursos/universidades.

### 3. Marketplace de Mentores
- Listagem de universitários/profissionais disponíveis.
- Sistema de agendamento, reviews, pagamentos (Stripe).
- Videochamada/chat integrado.

### 4. Painel PRO para Escolas
- Dashboard para professores/acesso a relatórios.
- Ferramentas de acompanhamento e exportação de PDFs.

### 5. Upsells e Produtos Digitais
- Geração automática de relatórios PDF personalizados.
- Mini-cursos em vídeo.

---

## 💰 Modelo de Monetização

- **Freemium para alunos:** Teste de perfil e recomendações básicas grátis.
- **Plano PRO/PREMIUM:** Subscrição mensal/anual ou pack único.
- **Marketplace:** Comissão sobre chamadas pagas.
- **Licenças para escolas:** Acesso PRO para colégios/escolas.
- **Upsells:** PDFs, cursos, workshops.

---

## 🛠️ Como Começar

### 1. Clonar o repositório

```bash
git clone https://github.com/seu-usuario/decide-futuro.git
cd decide-futuro
```

### 2. Instalar dependências

```bash
cd frontend
npm install
cd ../backend
npm install
```

### 3. Configurar variáveis de ambiente

- `.env` no backend (DB, Stripe, Auth, etc.)
- `.env` no frontend (API_URL, etc.)

### 4. Iniciar o projeto

```bash
# Backend
cd backend
npm run dev

# Frontend
cd ../frontend
npm run dev
```

---

## 📚 Roadmap de Desenvolvimento

1. **MVP**
   - Teste de perfil e recomendação de cursos
   - Simulador DGES básico
   - Autenticação de utilizadores

2. **Marketplace**
   - Listagem e agendamento de mentores
   - Integração de pagamentos e videochamadas

3. **Painel PRO para Escolas**
   - Dashboards, relatórios, exportação PDF

4. **Upsells e Parcerias**
   - Relatórios automáticos, mini-cursos, integrações B2B2C

---

## 🤝 Contribuição

1. Faça um fork do projeto
2. Crie uma branch (`git checkout -b feature/nome-feature`)
3. Commit as suas alterações (`git commit -am 'feat: nova feature'`)
4. Push para a branch (`git push origin feature/nome-feature`)
5. Abra um Pull Request

---

## 📄 Licença

MIT

---

Se quiser adaptar o guia para um stack diferente ou incluir exemplos de código/configuração, é só pedir!
