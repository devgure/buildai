# BuildBrainOS - AI Co-Pilot for Construction Execution

BuildBrainOS is a proactive AI agent ecosystem that automates the "invisible work" of construction. It serves General Contractors (GCs), Subcontractors, and Superintendents by providing intelligent automation for project management, compliance, safety, and payments.

## 🚀 Vision

"Procore stores data. BuildBrain thinks."

BuildBrainOS eliminates 70-80% of administrative overhead in construction by:
- Auto-scheduling subcontractors with GPS verification
- Predicting RFIs and change orders before delays occur
- Ensuring compliance with real-time insurance validation
- Providing voice-activated mobile assistance
- Matching bids intelligently via AI
- Accelerating payments with AI-verified work completion

## 🏗️ Architecture Overview

### Three-Layer Stack

1. **The "OS" – Execution & Compliance Engine** (Core SaaS)
   - Blueprint Intelligence Agent
   - Contract & Compliance Agent
   - Subcontractor Co-Pilot
   - RFI & Change Order Predictor
   - Safety Monitor
   - Voice Interface

2. **The "Wedge" – Smart Bidding & Submittals Marketplace**
   - BidBrain AI Matcher
   - Private Bid Portal
   - AI Scoring System

3. **The "Bank" – Embedded Fintech & Insurance**
   - PayBrain (Dynamic Factoring)
   - SafeRate Insurance

## 🛠️ Tech Stack

### Frontend
- **Mobile App**: React Native + Expo (iOS/Android)
- **Web Mobile**: React + Vite (PWA for tablets/field)
- **Web Desktop**: Next.js 14 (Admin Portal)

### Backend
- **API Gateway**: Kong (Node.js)
- **Microservices**: NestJS (TypeScript)
- **AI Agents**: FastAPI (Python)
- **Orchestration**: Temporal.io + LangGraph

### Data
- **Database**: MongoDB with Prisma ORM
- **Vector DB**: Qdrant for RAG
- **Cache**: Redis
- **File Storage**: AWS S3

### AI/ML
- **Reasoning**: Llama 3.1 70B (via Groq/vLLM)
- **Vision**: Qwen-2.5-VL
- **Orchestration**: LangGraph

### Infrastructure
- **Containerization**: Docker
- **Orchestration**: Kubernetes
- **Cloud**: AWS (EKS, S3, CloudFront)
- **Monitoring**: Prometheus, Grafana, Sentry

## 📊 Business Model

### Revenue Streams
- **Core SaaS**: $40/user/month (min 50 users) → $20M ARR
- **Bid Marketplace**: $500–$5K per awarded bid → $50M ARR
- **PayBrain**: 1% fee on verified payments → $50M ARR
- **SafeRate**: 15% commission on premiums → $30M ARR
- **Enterprise API**: $10k–$100k/year → $5M ARR

**Total ARR Projection**: Year 1: $8M → Year 5: $322M+

## 🎯 MVP Scope

### Core Features
1. **User Authentication & Profiles** (GCs, Subs, Supers)
2. **Project Management** (CRUD operations)
3. **Blueprint Upload & Basic OCR** (Text extraction)
4. **Bid Marketplace** (Post bids, apply, basic matching)
5. **Compliance Upload** (Insurance docs, basic validation)
6. **Safety Logging** (Photo upload, basic analysis)
7. **Payment Processing** (Stripe integration)
8. **Mobile App** (Basic navigation, offline sync)
9. **Admin Dashboard** (User/Project management)

### AI Features (MVP)
- Basic blueprint text extraction
- Simple bid matching algorithm
- OCR for compliance documents
- Basic safety photo classification

## 🚀 Getting Started

### Prerequisites
- Node.js 18+
- Python 3.9+
- Docker & Docker Compose
- MongoDB
- Redis

### Local Development Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-org/buildbrainos.git
   cd buildbrainos
   ```

2. **Environment Setup**
   ```bash
   cp env.example .env
   # Edit .env with your configuration
   ```

3. **Start Infrastructure**
   ```bash
   make infra-up
   ```

4. **Install Dependencies**
   ```bash
   make install
   ```

5. **Run Migrations**
   ```bash
   make migrate
   ```

6. **Start Services**
   ```bash
   make dev
   ```

### Development Commands

```bash
# Start all services
make dev

# Run tests
make test

# Build for production
make build

# Deploy to staging
make deploy-staging

# Clean up
make clean
```





## 📁 Project Structure

```
buildbrainos/
├── client/                       # Multi-platform UI
│   ├── mobile/                   # React Native + Expo
│   ├── web-mobile/               # PWA (React + Vite)
│   └── web-desktop/              # Admin Portal (Next.js)
├── gateway/                      # Kong API Gateway
├── services/                     # NestJS Microservices
│   ├── auth-service/
│   ├── user-service/
│   ├── project-service/
│   ├── document-service/
│   ├── compliance-service/
│   ├── marketplace-service/
│   ├── payment-service/
│   ├── notification-service/
│   └── analytics-service/
├── ai-agents/                    # Python FastAPI Microservices
│   ├── blueprint-agent/
│   ├── safety-agent/
│   ├── compliance-ocr-agent/
│   ├── bid-scraper-agent/
│   └── scheduler-agent/
├── orchestration/                # Temporal.io + LangGraph
├── data/                         # Data Layer
│   ├── mongodb/                  # Prisma schema
│   ├── qdrant/                   # Vector DB
│   └── redis.conf
├── infra/                        # Infrastructure as Code
├── monitoring/                   # Observability
├── admin-dashboard/             # Next.js Web Portal
├── tests/                        # Testing Suite
└── scripts/                      # Deployment Scripts
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is proprietary software. All rights reserved.

## 📞 Contact

For questions or partnerships, contact: hello@buildbrainos.com

---

**BuildBrainOS** – The AI Operating System for Construction Execution

Implement all NestJS microservices (auth, user, project, document, compliance, marketplace, payment, notification, analytics).
Create shared types package for type consistency.
Implement Python FastAPI AI agents.
Build React Native mobile app with Expo.
Create PWA web-mobile app with React + Vite.
Build admin dashboard with Next.js.
Set up Kong API gateway.
Implement Temporal workflows.
Configure Docker Compose for local dev.
Set up monitoring stack.
Create tests (unit, integration, e2e).
Write deployment scripts.
Create Makefile with common commands.
Set up environment variables and configuration.



