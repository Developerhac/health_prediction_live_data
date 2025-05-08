# Health Prediction Project Structure

## Project Overview
This is a full-stack health prediction application built with Next.js (frontend) and Python/Flask/Django (backend).

## Complete Project Structure

### Frontend Structure
```
📁 Root Directory
├── 📁 app/                    # Main application directory
│   ├── 📁 health-risk/       # Health risk assessment pages
│   ├── 📁 dashboard/         # Dashboard pages
│   ├── 📁 admin/            # Admin interface pages
│   ├── 📁 about/            # About page
│   ├── 📁 shared-results/   # Shared results pages
│   ├── 📁 predict/          # Prediction pages
│   ├── 📁 api/              # API routes
│   ├── 📄 page.tsx          # Home page
│   ├── 📄 layout.tsx        # Root layout
│   └── 📄 globals.css       # Global styles
│
├── 📁 components/            # Reusable components
│   ├── 📁 ui/               # UI components (extensive collection)
│   │   ├── 📄 accordion.tsx
│   │   ├── 📄 alert.tsx
│   │   ├── 📄 avatar.tsx
│   │   ├── 📄 button.tsx
│   │   ├── 📄 calendar.tsx
│   │   ├── 📄 chart.tsx
│   │   ├── 📄 dialog.tsx
│   │   ├── 📄 form.tsx
│   │   ├── 📄 input.tsx
│   │   ├── 📄 sidebar.tsx
│   │   └── [many more UI components...]
│   ├── 📄 premium-health-risk-chart.tsx
│   └── 📄 theme-provider.tsx
│
├── 📁 lib/                   # Utility functions
│   ├── 📄 data-utils.ts     # Data manipulation utilities
│   ├── 📄 validation.ts     # Form validation
│   ├── 📄 excel-utils.ts    # Excel file handling
│   └── 📄 utils.ts          # General utilities
│
├── 📁 hooks/                 # Custom React hooks
│   ├── 📄 use-toast.ts      # Toast notification hook
│   └── 📄 use-mobile.tsx    # Mobile detection hook
│
├── 📁 styles/               # Styling files
│   └── 📄 globals.css       # Global styles
│
├── 📁 public/               # Static assets
│   ├── 📄 placeholder.svg
│   ├── 📄 placeholder.jpg
│   ├── 📄 placeholder-user.jpg
│   ├── 📄 placeholder-logo.svg
│   └── 📄 placeholder-logo.png
│
├── 📄 premium-pie-chart.tsx # Pie chart component
├── 📄 package.json          # Dependencies and scripts
├── 📄 package-lock.json     # Dependency lock file
├── 📄 pnpm-lock.yaml        # PNPM lock file
├── 📄 next.config.mjs       # Next.js configuration
├── 📄 postcss.config.mjs    # PostCSS configuration
├── 📄 tailwind.config.ts    # Tailwind configuration
├── 📄 tsconfig.json         # TypeScript configuration
├── 📄 components.json       # Components configuration
└── 📄 .gitignore           # Git ignore rules
```

### Backend Structure
```
📁 python/
├── 📁 django_app/           # Django application
│   ├── 📄 views.py          # View functions
│   └── 📄 urls.py           # URL routing
│
├── 📄 app.py                # Main Flask application
├── 📄 predict.py            # Prediction model
├── 📄 requirements.txt      # Python dependencies
└── 📄 vercel.json          # Vercel deployment config
```

## Key Features and Components

1. **UI Components**: Extensive collection of reusable UI components in `components/ui/`
2. **Utility Functions**: Data handling, validation, and Excel operations in `lib/`
3. **Custom Hooks**: Toast notifications and mobile detection in `hooks/`
4. **Static Assets**: Placeholder images and logos in `public/`
5. **Backend Services**: Flask and Django applications for API and business logic
6. **Machine Learning**: Health prediction model in `predict.py`

## Setup Instructions

### Frontend Setup
```bash
# Install dependencies
npm install --legacy-peer-deps

# Run development server
npm run dev
```

### Backend Setup
```bash
# Navigate to python directory
cd python

# Create virtual environment
python -m venv venv

# Activate virtual environment
# Windows:
.\venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run Flask application
python app.py
```

## Technologies Used
- Frontend: Next.js, TypeScript, Tailwind CSS
- Backend: Python, Flask, Django
- Machine Learning: scikit-learn
- Data Visualization: Recharts
- UI Components: Radix UI 