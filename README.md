# CvGo — Deploy no Vercel

## Como subir

### 1. Suba para o GitHub
- Crie um repositório novo em github.com
- Faça upload de todos os arquivos desta pasta

### 2. Deploy no Vercel
- Acesse vercel.com
- Clique em "Add New Project"
- Conecte seu repositório GitHub
- Clique em "Deploy"

### 3. Configure a variável de ambiente
- No painel do Vercel, vá em Settings → Environment Variables
- Adicione:
  - Name: `GROQ_KEY`
  - Value: `gsk_SuaChaveAqui`

### 4. Pronto!
Seu app estará em: `https://cvgo.vercel.app`

## Estrutura
```
cvgo-vercel/
├── api/
│   ├── ai.py        # Proxy seguro para o Groq (chave protegida)
│   └── extract.py   # Extração de PDF/DOCX via servidor
├── public/
│   └── index.html   # Frontend do app
├── requirements.txt  # Dependências Python
└── vercel.json       # Configuração do Vercel
```
