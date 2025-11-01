🚀 RefreshFlow AI - Website Content Refresher

**with LangGraph + AI**

🌐 **See the Live Application**: https://ai-website-content-refresher-web.vercel.app/

An AI-powered content management platform that audits your website, generates SEO-optimized and accessibility-compliant content, runs A/B experiments, and ships changes via Git PRs or CMS drafts—all while staying true to your brand voice and guidelines.

## ✨ What is RefreshFlow AI?

RefreshFlow AI is your AI copilot for keeping website content fresh, accurate, and on-brand. It combines intelligent crawling, RAG-grounded content generation, and automated optimization to transform content workflows from weeks to hours.

**Core Capabilities:**

- 🕷️ **Smart Crawling**: Inventories pages, blocks, and detects templates automatically
- 🧠 **Brand-Aware AI**: RAG-grounded generation with your style guides, product docs, and FAQs
- ✍️ **Content Generation**: Page and block-level rewrites with citations and multiple tone presets
- 🔍 **SEO Optimization**: AI-powered analysis, title/meta rewrites, internal linking, and schema markup
- ♿ **Accessibility**: WCAG compliance suggestions, alt text generation, and contrast fixes
- 🧪 **A/B Testing**: Variant generation with hypotheses and export to Optimizely/VWO/GA4
- 🌍 **Localization**: Multi-language support with cultural adaptation and hreflang management
- 🔐 **Governance**: Side-by-side diffs, approval workflows, and reviewer checklists
- 🚢 **Publishing**: Git PR export or direct CMS draft push with review flows

## 💡 Benefits

**Speed**: Reduce content refresh cycles from weeks to hours—audit and generate updates in minutes, not days.

**Consistency**: Enforce brand voice and messaging across large sites with AI that learns from your guidelines.

**Growth**: Improve organic CTR and search rankings with AI-optimized titles, meta descriptions, and content structure.

**Compliance**: WCAG-aware suggestions and bias-aware phrasing reduce accessibility and legal risks.

**Efficiency**: Automated workflows free up content teams to focus on strategy instead of repetitive updates.

**Transparency**: Citation-backed content ensures accuracy and provides clear audit trails for claims.

## 🧭 Where This Can Be Applied

- 📘 **Documentation sites**: Keep technical docs, API references, and knowledge bases current
- 🛍️ **Ecommerce**: Scale product descriptions, category pages, and seasonal campaigns
- 🧩 **Marketing websites**: Refresh landing pages, blog posts, and conversion funnels
- 🌍 **Multi-region sites**: Manage localized content with cultural adaptation and hreflang
- 🏢 **Enterprise content**: Maintain compliance, brand consistency, and governance at scale
- 📰 **Publishing**: Update evergreen content and optimize for search visibility

## 🤖 AI Orchestration — LangGraph + CrewAI

RefreshFlow AI uses **LangGraph** as the primary orchestrator for deterministic, safety-critical pipelines (crawl → embed → retrieve → draft → SEO/accessibility analysis → publish). For workflows requiring multi-agent collaboration, we optionally leverage **CrewAI** for role-driven handoffs.

**Why LangGraph-first:**

- 👣 **Deterministic execution**: Reproducible pipelines with clear state management and recovery
- 🔁 **Fine-grained control**: Retry logic, conditional branching, and node-level tracing
- 🧵 **Observability**: Seamless integration with OpenTelemetry and job queues

**When CrewAI adds value:**

- 👥 **Multi-agent reviews**: Editorial handoffs with distinct roles (writer, editor, compliance)
- 🛠️ **Tool-driven research**: Autonomous agents for complex information gathering

### Framework Comparison

| Framework | Paradigm | Best For | Key Strengths | Learning Curve |
|---|---|---|---|---|
| **LangGraph** ✅ | State graph orchestration | Safety-critical flows | Deterministic, retries, branching, memory | Moderate |
| **CrewAI** | Multi-agent crews | Team-of-agents workflows | Role clarity, task planning, handoffs | Moderate |
| **LangChain Agents** | Single agent + tools | Quick prototyping | Large tool ecosystem, simple setup | Low |
| **AutoGen** | Agent-to-agent chat | Research & brainstorming | Multi-turn negotiation patterns | Moderate |
| **Semantic Kernel** | Skills + planners | Microsoft ecosystem | .NET first-class, Graph/Office integration | Moderate |

*All frameworks are capable—we chose LangGraph for control and reproducibility, with CrewAI for multi-agent scenarios.*

## 🚀 Quick Start

### Prerequisites

- **Node.js** 18+ and **npm** 9+
- **Python** 3.11+
- **PostgreSQL** 15+ with pgvector extension
- **Redis** 7+
- **OpenAI API Key** (for AI generation)


## 🏗️ Tech Stack

### Frontend
- **Next.js 14** with App Router and TypeScript
- **Tailwind CSS** for styling with dark mode support
- **React Context + hooks** for state management
- **WebSockets** for real-time progress updates
- **Playwright** for E2E testing

### Backend
- **FastAPI** with async support and WebSocket endpoints
- **Python 3.11+** with type hints throughout
- **SQLAlchemy** ORM with Alembic migrations
- **PostgreSQL 15+** with pgvector for embeddings
- **Redis** for caching and job queues
- **Structured logging** with monitoring hooks

### AI & ML
- **LangGraph**: Pipeline orchestration (crawl, embed, retrieve, draft, analyze)
- **LangChain**: RAG retrievers, document loaders, and tool integrations
- **OpenAI GPT-4**: Content generation and optimization
- **Anthropic Claude**: Long-form reasoning and analysis
- **pgvector**: Vector similarity search for brand knowledge retrieval
- **Sentence Transformers**: Text embedding models

### Infrastructure
- **Vercel**: Frontend hosting with edge functions
- **Railway/Render**: Backend API and worker deployment
- **Docker**: Containerization for consistent environments
- **JWT**: Authentication with refresh tokens
- **Prometheus**: Metrics and observability

## 🎯 Key Features

### 🔍 Smart Crawling & Inventory
- Automatic sitemap discovery and intelligent page detection
- Content block extraction with template recognition
- Broken link detection and orphan page identification
- Real-time WebSocket progress updates

### 🧠 Brand-Aware Content Generation
- RAG-grounded AI trained on your style guides and product documentation
- Citation-backed content for accuracy and audit trails
- Multi-tone presets: executive, friendly, concise, technical
- Page-level and block-level rewrites with context awareness

### 🔍 SEO Analysis & Optimization
- AI-powered SEO scoring with actionable recommendations
- Automated title/meta rewrites and H1-H3 structure optimization
- Internal link suggestions based on site context
- Schema markup (JSON-LD) and rich snippet generation
- Canonical URL and hreflang tag management

### ♿ Accessibility & Compliance
- WCAG 2.1 compliance analysis with severity ratings
- AI-generated alt text for images
- Contrast and readability optimization
- Link purpose clarity and keyboard navigation checks
- Bias-aware language suggestions

### 🧪 A/B Testing & Experimentation
- AI-powered variant generation with clear hypotheses
- Export to Optimizely, VWO, and Google Optimize
- Automatic minimum sample size calculation
- Statistical significance tracking

### 🌍 Localization & i18n
- Multi-language content generation with cultural adaptation
- Locale-specific formatting (dates, currency, measurements)
- hreflang tag management for regional SEO
- Translation consistency across pages

### 🔐 Governance & Approval Workflows
- Side-by-side diff viewer for content changes
- Multi-step approval routes (Marketing → Legal → Brand)
- Reviewer checklists and comment threads
- Audit logs with user attribution

### 🚢 Publishing & Integration
- Git PR export with formatted commit messages
- Direct CMS draft push (Contentful, Sanity, WordPress)
- Bulk operations for site-wide updates
- Rollback and version history

## 📊 Performance & Impact

- **80-90% faster**: Content refresh cycles reduced from weeks to hours
- **Higher CTR**: Improved organic click-through rates via optimized titles and meta descriptions
- **Zero performance impact**: Content-only changes maintain Core Web Vitals scores
- **Reduced compliance risk**: Citation-backed claims and approval workflows
- **Team efficiency**: Free content teams from repetitive tasks to focus on strategy


## 🚀 Deployment

### Frontend (Vercel)
Automatic deployment via GitHub integration. Configure environment variables in Vercel dashboard:
- `NEXT_PUBLIC_API_URL`: Backend API endpoint
- `NEXT_PUBLIC_WS_URL`: WebSocket endpoint

### Backend (Railway/Render)
Deploy from GitHub with automatic Docker builds. Required environment variables:
- `DATABASE_URL`: PostgreSQL connection string with pgvector
- `REDIS_URL`: Redis connection string
- `OPENAI_API_KEY`: OpenAI API key (optional fallback)
- `JWT_SECRET`: Secret for token signing

### Database Migrations
```bash
cd apps/api
alembic upgrade head    # Apply migrations
alembic revision --autogenerate -m "description"  # Create migration
```

## 📚 Documentation & Resources

- **[Live Application](https://ai-website-content-refresher-web.vercel.app/)**: Try the platform in action
- **[API Specification](docs/API_SPEC.md)**: Complete REST API documentation
- **[Repository Map](docs/REPO_MAP.md)**: Codebase structure and navigation guide
- **[Project Brief](docs/PROJECT_BRIEF.md)**: Requirements and technical specifications

## 🔒 Security & Credentials

### Authentication
- JWT-based authentication with refresh token rotation
- Role-based access control (RBAC) for multi-tenant environments
- Input validation and sanitization on all endpoints
- Rate limiting and DDoS protection

### API Key Management
- **LLM Keys (OpenAI/Anthropic)**: User-supplied keys via in-app modal, stored in sessionStorage only, sent per-request via headers (`x-openai-key`, `x-anthropic-key`). Backend uses keys in-memory and never persists them.
- **CMS/Git Connectors**: Server-managed tokens via environment variables, gated by `ENABLE_EXTERNAL_CONNECTORS=true`.
- **Analytics (GA4/GSC)**: Service account credentials configured via environment variables.
- **SSO (OIDC)**: Issuer/client configuration via environment; JWT role claims drive RBAC.

### Compliance
- Content Security Policy (CSP) headers
- CORS configuration for trusted origins
- Audit logs with user attribution
- GDPR-compliant data handling


## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Built With

RefreshFlow AI is powered by modern, production-grade technologies:

- **[Next.js](https://nextjs.org)** - React framework for the frontend
- **[FastAPI](https://fastapi.tiangolo.com)** - Python web framework for the API
- **[LangGraph](https://langchain.com/langgraph)** - AI pipeline orchestration
- **[LangChain](https://langchain.com)** - RAG and tool integrations
- **[OpenAI](https://openai.com)** - GPT-4 for content generation
- **[Anthropic](https://anthropic.com)** - Claude for reasoning tasks
- **[pgvector](https://github.com/pgvector/pgvector)** - Vector similarity search
- **[Tailwind CSS](https://tailwindcss.com)** - Utility-first CSS framework

---

**RefreshFlow AI** - Transform your website content with AI-powered intelligence.

© 2025 RefreshFlow AI • Created by Derril Filemon

[GitHub](https://github.com/refreshflow/refreshflow-ai) • [LinkedIn](https://www.linkedin.com/in/derril-filemon)
