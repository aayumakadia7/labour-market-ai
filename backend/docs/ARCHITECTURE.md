# National LMIS System Architecture & Directory Organization

The codebase is organized into high-level domain headings for scalability, maintainability, and seamless Vercel deployment:

```
├── frontend/                     # Primary Frontend Codebase
│   └── src/
│       ├── components/           # UI Components sorted by function
│       │   ├── navigation/       # Top Horizontal Nav, Mobile Slide-Over, Global Filters
│       │   ├── home/             # 3D Globe, Landing Page, Industrial Overlays
│       │   ├── mission/          # Mission Cockpit, National Telemetry Grid
│       │   ├── command/          # National Command Center View
│       │   ├── district/         # District War Room, Local Industry Voice
│       │   ├── sector/           # Sector Intelligence, AI Job Normaliser
│       │   ├── forecasting/      # Policy Scenario Simulator, Econometric Charts
│       │   ├── reports/          # Government Decision Support & Cabinet Hub
│       │   ├── saturation/       # Saturation Ranking & Trade Detail Drawers
│       │   ├── capacity/         # Capacity Target Setting & Reallocation
│       │   ├── talent/           # Talent Comparison View
│       │   ├── data/             # Data Observatory View
│       │   ├── copilot/          # AI Policy Copilot Chat Drawer
│       │   ├── modals/           # Action Plan, Cabinet Note, Command Palette Modals
│       │   ├── analytics/        # Choropleth Map, KPI Rows, Gap Charts
│       │   ├── api/              # API Explorer View
│       │   ├── settings/         # Accessibility & Settings View
│       │   ├── help/             # Methodology & Demand Index Explainability
│       │   └── common/           # Toasts, Animated Counter Utilities
│       ├── data/                 # Geographic Boundaries, Clusters & Pipelines
│       ├── hooks/                # Custom React Data & Analytics Hooks
│       ├── stores/               # Zustand Centralized Dashboard State
│       ├── styles/               # Global CSS & Tailwind Directives
│       ├── types/                # Strict TypeScript Interface Definitions
│       ├── utils/                # Number Formatters, Gap Scaling Math
│       ├── App.tsx               # Root Application Canvas
│       └── main.tsx              # DOM Hydration Entry Point
│
└── backend/                      # Dual-Runtime Backend (Express & FastAPI)
    ├── ai/                       # ML Models, Pipelines, Training & Prompts
    ├── api/                      # Edge Functions & Serverless Handlers
    ├── database/                 # PostgreSQL + TimescaleDB Schemas & Seeds
    ├── docs/                     # System & Deployment Architecture Docs
    ├── routes/                   # REST API Endpoints (/telemetry, /briefs, /models)
    ├── scripts/                  # ML Pipelines & Model Fine-Tuning Scripts
    ├── services/                 # Hugging Face AI & Telemetry Services
    ├── config.py                 # FastAPI Configuration & Settings
    ├── main.py                   # FastAPI Analytical Application Entry Point
    ├── server.ts                 # Express Application Gateway Server
    ├── package.json              # Backend Node.js Package Configuration
    └── tsconfig.json             # Backend TypeScript Configuration
```
