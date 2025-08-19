# ⚡ N8N Workflow Coleção & Documentação

Uma coleção profissionalmente organizada de **2,053 n8n workflows** com um sistema de documentação extremamente rápido que fornece recursos instantâneos de pesquisa, análise e navegação.

> **⚠️ AVISO IMPORTANTE (14 de agosto de 2025): O histórico do repositório foi reescrito para
fins de conformidade com a DMCA. Se você tiver um fork ou clone local, consulte [Issue #X](https://github.com/Zie619/n8n-workflows/issues)  para obter instruções sobre como sincronizar sua cópia.

## 🚀 ** NOVO: Sistema de Documentação de Alto Desempenho**
**Experimente uma melhoria de desempenho de 100x em relação à documentação tradicional!**
### Início rápido - Sistema de documentação rápida
```bash
# Install dependencies
pip install -r requirements.txt

# Start the fast API server
python run.py

# Open in browser
http://localhost:8000
```

**Características:**
- ⚡ **Tempos de resposta abaixo de 100 ms** com pesquisa SQLite FTS5
- 🔍 ** Pesquisa instantânea de texto completo** com filtragem avançada
- 📱 ** Design responsivo** funciona perfeitamente em dispositivos móveis
- 🌙 **Temas claros/escuros** com detecção de preferências do sistema
- 📊 ** Estatísticas ao vivo**  365 integrações exclusivas, 29.445 total de nodes
- 🎯 **Categorização inteligente** por tipo de gatilho e complexidade
- 🎯 **Categorização de casos de uso** por nome de serviço mapeado para categorias
- 📄 **Visualização JSON sob demanda** e download
- 🔗 **Geração de diagrama de sereia** para visualização do fluxo de trabalho
- 🔄 **Nomenclatura de workflow em tempo real** com formatação inteligente

### Comparação de desempenho

|        Métrica            | Sistema antigo          | Novo Sistema  |        Melhoria           |
|--------------------------|-------------------------|---------------|---------------------------|
| **Tamanho do arquivo**   | 71MB HTML               | <100KB        | **700x menor**            |
| **Tempo de carregamento**| 10+ segundos            | <1 segundo    | **10x mais rápido**       |
| **Search**               | Só lado lado do cliente |Full-text FTS5 | **Instant**               |
| **Uso de memória**       | ~2GB RAM                | <50MB RAM     | **40x menos**             |
| **Supporte Mobile**      | Pobre                   | Excellente    | **Totalmente responsivo** |
---
## 📂 Organização do Repositório

### Coleção de Workflow
- **2,053 workflows** com nomes significativos e pesquisáveis
- **365 integrações exclusivas** em plataformas populares
- **29,445 total de nodes** com categorização profissional
- **Garantia de qualidade** Todos workflows analisados e categorizados

### Sistema de Nomenclatura Avançado ✨
Nosso sistema de nomenclatura inteligente converte nomes de arquivos técnicos em títulos legíveis:
- **Antes**: 2051_Telegram_Webhook_Automation_Webhook.json
- **Depois**: `Telegram Webhook Automation`
- **Nomes 100% significativos** com capitalização inteligente
- **Detecção automática de integração** a partir da análise de nós

### Categoria de caso de uso ✨

A interface de pesquisa inclui um filtro suspenso que permite navegar por mais de 2.000 workflows por categoria.

O sistema inclui um recurso de categorização automatizado que organiza os workflows por categorias de serviço para torná-los mais fáceis de descobrir e filtrar.

### Como funciona a categorização

1. ** Execute o script de categorização**
   ```
   python create_categories.py   ```

2. **Reconhecimento de nome de serviço**
   O script analisa cada nome de arquivo JSON do workflow para identificar nomes de serviço reconhecidos (por exemplo, "Twilio", "Slack", "Gmail" etc.)

3. ** Mapeamento de Categoria**
   Cada nome de serviço reconhecido é correspondido à sua categoria correspondente usando as definições em  `context/def_categories.json`. Por exemplo:
   - Twilio → Comunicação e Mensagens
   - Gmail → Comunicação e Mensagens
   - Airtable → Processamento e Análise de Dados
   - Salesforce → CRM e Vendas

4. **Search Geração de categorias**
  O script produz um `search_categories.json`  arquivo que contém os dados do workflow categorizados

5. **Filter Interface**
    Os usuários podem então filtrar workflows  por categoria na interface de pesquisa, tornando mais fácil encontrar workflows  para casos de uso específicos

### Categorias disponíveis

O sistema de categorização inclui as seguintes categorias principais:
- AI Agent Development
- Business Process Automation
- Cloud Storage & File Management
- Communication & Messaging
- Creative Content & Video Automation
- Creative Design Automation
- CRM & Sales
- Data Processing & Analysis
- E-commerce & Retail
- Financial & Accounting
- Marketing & Advertising Automation
- Project Management
- Social Media Management
- Technical Infrastructure & DevOps
- Web Scraping & Data Extraction

### Contribuir Categorias

Você pode ajudar a expandir a categorização adicionando mais mapeamentos de serviço para categoria (por exemplo, Twilio → Comunicação e Mensagens) em context/defs_categories.json.

Muitos workflow de arquivos JSON são convenientemente nomeados com o nome do serviço, geralmente separados por sublinhados (_).


---

## 🛠  Instruções de uso

### Opção 1: Sistema rápido moderno (recomendado)
```bash
# Clone repository
git clone <repo-url>
cd n8n-workflows

# Install Python dependencies
pip install -r requirements.txt

# Start the documentation server
python run.py

# Browse workflows at http://localhost:8000
# - Instant search across 2,053 workflows
# - Professional responsive interface
# - Real-time workflow statistics
```

### Opção 2: Modo de Desenvolvimento
```bash
# Start with auto-reload for development
python run.py --dev

# Or specify custom host/port
python run.py --host 0.0.0.0 --port 3000

# Force database reindexing
python run.py --reindex
```

### Importar Workflows para o n8n
```bash
# Use the Python importer (recommended)
python import_workflows.py

# Or manually import individual workflows:
# 1. Open your n8n Editor UI
# 2. Click menu (☰) → Import workflow
# 3. Choose any .json file from the workflows/ folder
# 4. Update credentials/webhook URLs before running
```

---

## 📊 Estatísticas de fluxo de trabalho

### Estatísticas atuais da coleção
- **Total Workflows**: 2,053 workflows de automação
- **Workflows Ativos**: 215 (taxa de atividade de 10,5%)
- **Total Nodes**: 29,445 (média 14.3 nodes por workflow)
- **Integrações exclusivas**: 365 serviços e APIs diferentes
- **Database**: SQLite com pesquisa de texto completo FTS5

### Distribuição de gatilhos
- **Complexo**: 831 workflows (40,5%) - Sistemas multi-gatilho
- **Webhook**: 519 workflows (25,3%) - automações acionadas por API
- **Manual**: 477 workflows (23,2%) - workflows iniciados pelo usuário
- **Agendado**: 226 workflows (11,0%) - Execuções baseadas em tempo

### Análise de Complexidade
- **Baixo (≤5 nodes)**: ~35% - Automações simples
- **Médio (6-15 nodes)**: ~45% - workflows padrão
- **Alto (16+ nodes)**: ~20% - Sistemas enterprise complexos

### Integrações populares
Principais serviços por frequência de uso:
- **Comunicação**: Telegram, Discord, Slack, WhatsApp
- **Cloud Storage**: Google Drive, Google Sheets, Dropbox
- **Databases**: PostgreSQL, MySQL, MongoDB, Airtable
- **AI/ML**: OpenAI, Anthropic, Hugging Face
- **Development**: HTTP Request, Webhook, GraphQL

---

## 🔍 Recursos de pesquisa avançada

### Categorias de pesquisa inteligente
Nosso sistema categoriza automaticamente os workflows em 12 categorias de serviço:

#### Categorias disponíveis:
- **messaging**: Telegram, Discord, Slack, WhatsApp, Teams
- **ai_ml**: OpenAI, Anthropic, Hugging Face 
- **database**: PostgreSQL, MySQL, MongoDB, Redis, Airtable
- **email**: Gmail, Mailjet, Outlook, SMTP/IMAP
- **cloud_storage**: Google Drive, Google Docs, Dropbox, OneDrive
- **project_management**: Jira, GitHub, GitLab, Trello, Asana
- **social_media**: LinkedIn, Twitter/X, Facebook, Instagram
- **ecommerce**: Shopify, Stripe, PayPal
- **analytics**: Google Analytics, Mixpanel
- **calendar_tasks**: Google Calendar, Cal.com, Calendly
- **forms**: Typeform, Google Forms, Form Triggers
- **development**: Webhook, HTTP Request, GraphQL, SSE

### Exemplos de uso de API
```bash
# Search workflows by text
curl "http://localhost:8000/api/workflows?q=telegram+automation"

# Filter by trigger type and complexity
curl "http://localhost:8000/api/workflows?trigger=Webhook&complexity=high"

# Find all messaging workflows
curl "http://localhost:8000/api/workflows/category/messaging"

# Get database statistics
curl "http://localhost:8000/api/stats"

# Browse available categories
curl "http://localhost:8000/api/categories"
```

---

## 🏗 Arquitetura Técnica

### Modern Stack
- **SQLite Database** - Pesquisa de texto completo FTS5 com 365 integrações indexadas
- **FastAPI Backend** - API RESTful com documentação automática OpenAPI
- **Responsive Frontend** - HTML5 moderno com CSS/JavaScript incorporado
- **Smart Analysis** - Categorização e nomenclatura automáticas do workflow
### Principais características
- **Change Detection** - hash MD5 para reindexação eficiente
- **Background Processing** - - Análise de workflow sem bloqueio
- **Compressed Responses** - Gzip middleware para velocidade ideal
- **Error Handling** - Degradação elegante e registro abrangente
- **Mobile Optimization** - Design de interface amigável ao toque

### Database Desempenho
```sql
-- Optimized schema for lightning-fast queries
CREATE TABLE workflows (
    id INTEGER PRIMARY KEY,
    filename TEXT UNIQUE,
    name TEXT,
    active BOOLEAN,
    trigger_type TEXT,
    complexity TEXT,
    node_count INTEGER,
    integrations TEXT,  -- JSON array of 365 unique services
    description TEXT,
    file_hash TEXT,     -- MD5 for change detection
    analyzed_at TIMESTAMP
);

-- Full-text search with ranking
CREATE VIRTUAL TABLE workflows_fts USING fts5(
    filename, name, description, integrations, tags,
    content='workflows', content_rowid='id'
);
```

---

## 🔧 Configuração e requisitos

### Requisitos do sistema
- **Python 3.7+** - Para executar o sistema de documentação
- **Browser Moderno** - Chrome, Firefox, Safari, Edge
- **50MB Storage** - Para database e índices SQLite
- **n8n Instance** - Para importar e executar workflows

### Instalação
```bash
# Clone repository
git clone <repo-url>
cd n8n-workflows

# Install dependencies
pip install -r requirements.txt

# Start documentation server
python run.py

# Access at http://localhost:8000
```

### Configurar Desenvolvimento
```bash
# Create virtual environment
python3 -m venv .venv
source .venv/bin/activate  # Linux/Mac
# or .venv\Scripts\activate  # Windows

# Install dependencies
pip install -r requirements.txt

# Run with auto-reload for development
python api_server.py --reload

# Force database reindexing
python workflow_db.py --index --force
```

---

## 📋 Convenção de Nomenclatu

### Sistema de Formatação Inteligente
Nosso sistema converte automaticamente nomes de arquivos técnicos em nomes amigáveis:

```bash
# Automatic transformations:
2051_Telegram_Webhook_Automation_Webhook.json → "Telegram Webhook Automation"
0250_HTTP_Discord_Import_Scheduled.json → "HTTP Discord Import Scheduled"  
0966_OpenAI_Data_Processing_Manual.json → "OpenAI Data Processing Manual"
```

### Formato técnico
```
[ID]_[Service1]_[Service2]_[Purpose]_[Trigger].json
```

### Regras de Capitalização Inteligente
- **HTTP** → HTTP (not Http)
- **API** → API (not Api)  
- **webhook** → Webhook
- **automation** → Automation
- **scheduled** → Scheduled

---

## 🚀 Documentação da API

### Core Endpoints
- `GET /` - Main workflow browser interface
- `GET /api/stats` - Database statistics and metrics
- `GET /api/workflows` - Search with filters and pagination
- `GET /api/workflows/{filename}` - Detailed workflow information
- `GET /api/workflows/{filename}/download` - Download workflow JSON
- `GET /api/workflows/{filename}/diagram` - Generate Mermaid diagram

### Advanced Search
- `GET /api/workflows/category/{category}` - Search by service category
- `GET /api/categories` - List all available categories
- `GET /api/integrations` - Get integration statistics
- `POST /api/reindex` - Trigger background reindexing

### Response Examples
```json
// GET /api/stats
{
  "total": 2053,
  "active": 215,
  "inactive": 1838,
  "triggers": {
    "Complex": 831,
    "Webhook": 519,
    "Manual": 477,
    "Scheduled": 226
  },
  "total_nodes": 29445,
  "unique_integrations": 365
}
```

---

## 🤝  Contribuind

### Adicionando novos Workflows
1. **Export workflow** como JSON do n8n
2. **Name descriptively** fseguindo o padrão estabelecido
3. **Add to workflows/** diretório
4. **Remove sensitive data** (credenciais, URLs pessoais)
5. **Run reindexing**  para atualizar o banco de dados


### Padrões de Qualidade
- ✅ O Workflow deve ser funcional e testado
- ✅ Remova todas as credenciais e dados confidenciais
- ✅ Siga a convenção de nomenclatura para consistência
- ✅ Verifique a compatibilidade com versões recentes do n8n
- ✅ Inclua descrições ou comentários significativos

---

## ⚠️ Notas importantes

### Segurança e Privacidade
- **Revisar antes de usar** - Todos os workflows são compartilhados no estado em que se encontram para fins educacionais
- **Atualizar credenciais** - Substituir chaves de API, tokens e webhooks
- **Teste com segurança** - Verifique primeiro no ambiente de desenvolvimento
- **Verifique as permissões** - Garanta os direitos de acesso adequados para integrações

### Compatibilidade
- **n8n Version** - Compatível com n8n 1.0+ (a maioria dos workflows)
- **Community Nodes** - Alguns workflows podem exigir instalações de nodes adicionais
- **API Changes** - Serviços externos podem ter atualizado suas APIs desde a criação
- **Dependencies** - Verifique as integrações necessárias antes de importar

---

## 📚 Recursos e Referências

### Workflow Sources
Esta coleção abrangente inclui workflows de:

- **N8n.io oficial** - Documentação e exemplos da comunidade
- **Repositórios GitHub** - Contribuições da comunidade de código aberto
- **Postagens de blog e tutoriais** - Padrões de automação do mundo real
- **Envios de usuários** - Fluxos de trabalho testados e verificados
- **Casos de uso empresarial** - Automação de processos de negócios

### Learn More
- [n8n Documentation](https://docs.n8n.io/) - Documentação oficial
- [n8n Community](https://community.n8n.io/) - Fórum e suporte da comunidade
- [Workflow Templates](https://n8n.io/workflows/) - Biblioteca oficial de modelos
- [Integration Docs](https://docs.n8n.io/integrations/) - Guias específicos de serviço

---

## 🏆  Conquistas do Projeto

### Transformação de Repositório
- **2,053 workflows** organizados e nomeados profissionalmente
- **365 integrações exclusivas** detectadas e categorizadas automaticamente
- **Nomes 100% significativos** (melhorados em relação aos padrões básicos de nomes de arquivos)
- **Perda zero de dados** durante o processo de renomeação inteligente
- **Pesquisa avançada** com 12 categorias de serviços


### Revolução de Desempenho
- **Pesquisa abaixo de 100ms** com indexação de texto completo SQLite FTS5
- **Filtragem instantânea** em 29.445 nós de fluxo de trabalho
- **Mobile-otimizado** design responsivo para todos os dispositivos
- **Estatísticas em tempo real** com consultas de banco de dados ao vivo
- **nterface profissional** com princípios modernos de UX

### Confiabilidade do sistema
- **Tratamento de erros robusto** com degradação suave
- **Detecção de alterações** para atualizações eficientes do banco de dados
- **Processamento em segundo plano** para operações não bloqueantes
- **Registro abrangente** para depuração e monitoramento
- **Pronto para produção** com middleware e segurança adequados

---
*Este repositório representa a coleção mais abrangente e bem organizada de workflows do N8N disponíveis, apresentando tecnologia de pesquisa de ponta e documentação profissional que torna a descoberta e o uso dos workflows uma experiência agradável.*


**🎯  Perfeito para : desenvolvedores, engenheiros de automação, analistas de negócios e qualquer pessoa que queira otimizar seus fluxos de trabalho com automações n8n comprovadas.





