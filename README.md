# Google Maps Grounding Demo

A modern web application demonstrating Google Maps integration with grounding capabilities, built with React, TypeScript, and Tailwind CSS.

## Tech Stack

- **React 19** - UI library
- **TypeScript** - Type-safe development
- **Vite** - Fast build tool and dev server
- **Tailwind CSS v4** - Utility-first CSS framework
- **shadcn/ui** - High-quality React components
- **pnpm** - Fast, disk space efficient package manager

## Project Structure

```
src/
├── components/         # React components
│   ├── ui/            # shadcn/ui components
│   ├── maps/          # Google Maps related components
│   └── layout/        # Layout components
├── hooks/             # Custom React hooks
├── lib/               # Utility functions
├── types/             # TypeScript type definitions
├── constants/         # Application constants
├── styles/            # Global styles
│   ├── index.css
│   └── tw-animate-css.css
├── App.tsx            # Main app component
└── main.tsx           # Application entry point
```

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- pnpm (v8 or higher)
- Google Maps API Key

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd google-maps-grounding-demo
```

2. Install dependencies:
```bash
pnpm install
```

3. Set up environment variables:
```bash
cp .env.example .env
```

4. Add your Google Maps API key to `.env`:
```env
VITE_GOOGLE_MAPS_API_KEY=your_api_key_here
```

### Development

Start the development server:
```bash
pnpm dev
```

The application will be available at `http://localhost:5173`

### Build

Build for production:
```bash
pnpm build
```

Preview the production build:
```bash
pnpm preview
```

## Code Quality

### Linting

Run ESLint to check for code quality issues:
```bash
pnpm lint
```

Auto-fix linting issues:
```bash
pnpm lint:fix
```

### Formatting

Format code with Prettier:
```bash
pnpm format
```

Check formatting without making changes:
```bash
pnpm format:check
```

## Adding shadcn/ui Components

Add new shadcn/ui components:
```bash
pnpm dlx shadcn@latest add <component-name>
```

Example:
```bash
pnpm dlx shadcn@latest add button
pnpm dlx shadcn@latest add card
pnpm dlx shadcn@latest add dialog
```

## VSCode Setup

### Recommended Extensions

- ESLint (`dbaeumer.vscode-eslint`)
- Prettier (`esbenp.prettier-vscode`)
- Tailwind CSS IntelliSense (`bradlc.vscode-tailwindcss`)

### Settings

The project includes VSCode settings in `.vscode/settings.json` that enable:
- Format on save
- Auto-fix ESLint issues on save
- Tailwind CSS IntelliSense
- Custom CSS directives support

## License

MIT
