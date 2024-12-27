# Brandock - AI-Powered Brand Development Platform

## Overview

Brandock is a sophisticated AI-powered platform designed to assist in brand development and strategy. It combines multiple specialized AI models to provide comprehensive branding insights and recommendations.

## Features

### AI Models

- **EthosAI**: Philosophical and ethical brand analysis
- **CultureAI**: Cultural and sociological analysis
- **PsycheAI**: Psychological brand analysis
- **NeuroAI**: Neuroscience-based brand insights
- **InsightAI**: Strategic brand insights
- **DataBrandAI**: Data-driven brand analysis
- **SymbolAI**: Brand symbolism and semiotics
- **EthnoAI**: Ethnographic brand research

### Core Functionality

- Multi-model conversations
- Project organization
- Resource library (prompts and ebooks)
- Premium features
- Daily usage limits for free users

## Technical Stack

- **Frontend**: React + TypeScript
- **Styling**: Tailwind CSS
- **Backend**: Supabase
- **Authentication**: Supabase Auth
- **Database**: PostgreSQL (via Supabase)

## Project Structure

```
src/
├── components/        # React components
│   ├── chat/         # Chat-related components
│   └── layout/       # Layout components
├── hooks/            # Custom React hooks
├── lib/              # Utility functions and configurations
├── pages/            # Page components
└── types/            # TypeScript type definitions

supabase/
└── migrations/       # Database migrations
```

## Database Schema

### Main Tables

- `users`: User profiles and settings
- `projects`: Project organization
- `chat_conversations`: Chat conversations
- `chat_messages`: Individual chat messages
- `ai_models`: Available AI models
- `conversation_models`: Links between conversations and models
- `resources`: Educational resources and prompts

## Security

- Row Level Security (RLS) policies
- Role-based access control
- Premium content restrictions

## Usage Limits

- Free users: Limited daily messages
- Premium users: Unlimited access

## Development

1. Install dependencies:
   ```bash
   npm install
   ```

2. Start development server:
   ```bash
   npm run dev
   ```

3. Build for production:
   ```bash
   npm run build
   ```

## Environment Variables

Required environment variables:
```
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Submit a pull request

## License

MIT License

Esse foi o prompt que enviamos ao Bolt.new para iniciar o projeto:

# Prompt para Desenvolvimento de Plataforma de Branding com IA

## Design Base
- Tema: Dark mode puro com fundo preto (#000000)
- Interface: Minimalista e elegante inspirada no Gemini
- Elementos visuais:
  - Cards com bordas significativamente arredondadas (border-radius: 16px)
  - Animações suaves nas transições
  - Efeito de hover sutil nos cards (leve aumento de opacidade)
- Toggle dark/light mode no header

## Estrutura da Interface

### Header
- Logo à esquerda
- Barra de busca central com ícone de lupa
- Toggle dark/light mode
- Avatar do usuário
- Notificações

### Layout Principal (3 Colunas)
1. Chat IA (Coluna Principal)
   - Campo de mensagem grande e minimalista
   - Resposta do assistente em cards arredondados
   - Sugestões de prompts em chips horizontais
   - Indicador de digitação animado

2. Resource Library (Segunda Coluna)
   - Cards arredondados para cada área científica:
     - Philosophy & Ethics
     - Sociology & Culture
     - Psychology
     - Neuroscience
     - Storytelling & Narratives
     - Data & Research

3. Tools & Templates (Terceira Coluna)
   - Brand Strategy
   - Identity Design
   - Brand Management
   - Campaign Planning

### Sistema de Acesso
- Freemium:
  - Chat básico
  - Biblioteca limitada
  - Templates básicos
  
- Premium:
  - Chat avançado com todas as especialidades
  - Biblioteca completa
  - Ferramentas avançadas
  - Exports personalizados
  - Análises detalhadas

## Funcionalidades Core

### Chat IA
- Interface clean e minimalista
- Sugestões contextuais em chips
- Histórico de conversas em sidebar colapsável
- Exportação de insights

### Biblioteca de Recursos
Organizada em cards arredondados por ciência:

1. Philosophy & Ethics
   - Brand Purpose
   - Value Systems
   - Ethical Guidelines
   - Cultural Impact

2. Sociology & Culture
   - Cultural Analysis
   - Social Trends
   - Consumer Behavior
   - Market Dynamics

3. Psychology
   - Archetypes
   - Behavioral Patterns
   - Consumer Motivation
   - Decision Making

4. Neuroscience
   - Attention Triggers
   - Memory Formation
   - Emotional Response
   - Sensory Branding

5. Storytelling & Narratives
   - Story Structures
   - Brand Voice
   - Content Strategy
   - Campaign Scripts

6. Data & Research
   - Market Analysis
   - Consumer Insights
   - Trend Reports
   - Performance Metrics

### Branding Tools
- Templates estratégicos
- Frameworks de análise
- Geradores de relatórios
- Planejadores de campanha

## Elementos de UI/UX

### Cards
- Background: rgba(255, 255, 255, 0.05)
- Border-radius: 16px
- Hover state: Sutil aumento de opacidade
- Transição: 0.3s ease-in-out

### Typography
- Headlines: SF Pro Display
- Body: Inter
- Weights: Regular (400), Medium (500), Bold (700)

### Cores
- Background: #000000
- Cards: rgba(255, 255, 255, 0.05)
- Text Primary: #FFFFFF
- Text Secondary: rgba(255, 255, 255, 0.7)
- Accent: #0066FF
- Success: #00C853
- Warning: #FFD600
- Error: #FF3D00

### Interações
- Feedback visual imediato
- Tooltips informativos
- Loading states minimalistas
- Microinterações suaves

## Fluxo de Navegação

1. Landing/Login
   - Tela clean com login/registro
   - Opções de plano (Freemium/Premium)

2. Onboarding
   - Tour guiado das funcionalidades
   - Seleção de áreas de interesse
   - Configuração inicial de preferências

3. Dashboard Principal
   - Chat IA centralizado
   - Acesso rápido à biblioteca
   - Tools em destaque

## Considerações Técnicas
- Componentização modular
- Performance otimizada
- Sistema de cache eficiente
- Sincronização em tempo real
- Responsividade total
- PWA ready

## Segurança
- Autenticação robusta
- Criptografia end-to-end
- Backup automático
- Controle de acesso granular
- Conformidade LGPD