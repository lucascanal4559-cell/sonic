# Sonic Vendas Premium — Sistema Completo Full-Stack

Sistema comercial de alta performance com loja virtual, painel administrativo multi-domínio, catálogo de redes sociais, divulgação de contatos e negócios com orçamento IA, sorteios com cotas e apuração Loteria Federal, roleta da sorte interativa, teste IPTV de 12 horas, central de notificações sonoras (Web Audio API), personalização de temas e fontes Google Fonts, e aprovação de comprovantes Pix.

---

## 🌐 Domínios Suportados (Multi-Domínio Integrado)
- **Site dos Clientes (Loja):** `https://sonicvendas.app`
- **Painel Administrativo:** `https://sonicvendasadm.app`
- O `src/middleware.ts` direciona automaticamente o visitante para a loja ou para o painel de acordo com o domínio acessado.

---

## 🔐 Credenciais Padrão do Administrador
- **URL de Login:** `/admin/login` (ou na raiz de `sonicvendasadm.app`)
- **E-mail:** `lucasgame988@gmail.com`
- **Senha:** `jogo1212`

---

## 🚀 Como Instalar e Rodar em Qualquer Hospedagem (Vercel, VPS, Railway, Render, Docker, etc.)

### 1. Pré-requisitos
- Node.js 18+ ou 20+
- PostgreSQL (local ou remoto, como Supabase, Neon, Railway, AWS RDS, etc.)

### 2. Instalação das Dependências
```bash
npm install
```

### 3. Configuração do `.env`
Crie ou edite o arquivo `.env` na raiz do projeto (use `.env.example` como base):
```env
DATABASE_URL=postgresql://postgres:postgres@127.0.0.1:5432/app_db

# URLs e Domínios
NEXT_PUBLIC_SITE_NAME="Sonic Vendas Premium"
NEXT_PUBLIC_SITE_URL="https://sonicvendas.app"
NEXT_PUBLIC_ADMIN_URL="https://sonicvendasadm.app"

# Chave Pix Oficial e WhatsApp Suporte
NEXT_PUBLIC_PIX_KEY="75981558007"
NEXT_PUBLIC_SUPPORT_PHONE="75981558007"

# Mercado Pago (Opcional)
MERCADO_PAGO_ACCESS_TOKEN=seu_access_token
MERCADO_PAGO_PUBLIC_KEY=sua_public_key
```

### 4. Sincronizar o Banco de Dados PostgreSQL
Execute o comando do Drizzle ORM para criar todas as tabelas automaticamente no seu PostgreSQL:
```bash
npx drizzle-kit push
```

### 5. Compilar e Iniciar em Produção
```bash
npm run build
npm start
```

---

## 📋 Funcionalidades Incluídas no Pacote

1. **Loja Virtual & Produtos:**
   - Vitrine moderna com garantia oficial da loja / fabricante configurável.
   - Categorias dinâmicas e pesquisa em tempo real.
   - Checkout completo com Pix e envio de comprovante com destaque visual pulsante.
2. **📱 Redes Sociais & Engajamento com Reposição:**
   - Instagram, TikTok, Kwai, YouTube, Facebook, Free Fire, Threads, Twitch, Spotify e TV por Assinatura.
   - Calculadora de orçamento em tempo real com chave Pix `75981558007`.
3. **👤 Divulgação de Contatos (R$ 1,00/dia):**
   - Perfis pessoais, foto, vídeo de 2 min, WhatsApp e contagem de cliques reais.
4. **💼 Divulgação de Vendas & Negócios:**
   - Lojas, empresas e marcas com **Orçamento Inteligente sugerido pela IA**.
   - Botão **IMPULSIONAR** com planos de destaque Topo (3d, 7d, 15d, 30d).
5. **🎯 Sorteios & Cotas (R$ 0,01 a R$ 0,50):**
   - Geração automática de códigos únicos sem repetição no servidor.
   - Apuração com vinculação oficial à Loteria Federal e revelação na Live do Instagram.
6. **🎡 Roleta da Sorte Interativa:**
   - Animação canvas, áudio sintetizado e fatias 100% editáveis no painel ADM.
7. **📺 IPTV Teste de 12 Horas:**
   - Solicitação pública e liberação com credenciais e cronômetro regressivo de 12 horas.
8. **👥 Grupos da Comunidade:**
   - WhatsApp, Telegram e Discord organizados por categorias com taxa mensal de R$ 10,00.
9. **🔊 Central de Notificações Sonoras (Web Audio API):**
   - 7 tipos de sons profissionais e harmônicos sintetizados sem falhas de áudio.
10. **🎨 Personalização Avançada de Fontes e Cores:**
    - Google Fonts dinâmico (Poppins, Inter, Montserrat, etc.), paleta de cores e imagem/vídeo de fundo.
11. **📄 Auditoria de Comprovantes Pix pelo ADM:**
    - Botões para o administrador aceitar ou rejeitar compras após conferência no banco.
12. **🚀 Roadmap de Novidades com Gerador IA:**
    - Digite qualquer ideia e a IA gera a especificação técnica completa.

---

© 2026 Sonic Vendas Premium. Todos os direitos reservados.
