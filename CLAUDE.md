# LifeKLine Development Guidelines

> React 19 + TypeScript + Vite 中国命理可视化项目

## Quick Reference

**Package Manager**: npm
**Build Tool**: Vite
**Framework**: React 19 + TypeScript

### Common Commands
```bash
# Development
npm run dev              # Start dev server (http://localhost:5173)
npm run build           # Production build
npm run preview         # Preview production build

# Code Quality
npx tsc --noEmit        # Type checking
npx prettier --write .  # Format code
```

## Project Structure

```
lifekline/
├── App.tsx              # Main application component
├── index.tsx           # Entry point
├── components/         # React components
├── services/           # API services
├── assets/             # Static assets
├── types.ts            # TypeScript types
├── constants.ts        # Constants and config
└── mock-data.json      # Mock data for development
```

## Tech Stack

- **Frontend**: React 19, TypeScript
- **Styling**: TailwindCSS
- **Charts**: Recharts
- **Build**: Vite 5
- **State**: React Hooks

## Development Conventions

### TypeScript
- Use strict mode
- Define types in `types.ts`
- Avoid `any` type
- Use interfaces for component props

### React
- Functional components only
- Use hooks (useState, useEffect, useMemo, etc.)
- Props destructuring
- Keep components small and focused

### Styling
- TailwindCSS utility classes
- Responsive design (mobile-first)
- Dark mode support if needed

### File Naming
- Components: PascalCase (e.g., `KLineChart.tsx`)
- Types: PascalCase interfaces (e.g., `interface ChartData {}`)
- Constants: UPPER_SNAKE_CASE

## Code Quality Standards

### Before Committing
- [ ] TypeScript compiles without errors (`npx tsc --noEmit`)
- [ ] Code is formatted (`npx prettier --write .`)
- [ ] Component renders without errors
- [ ] No console errors in browser

### Component Checklist
- [ ] TypeScript interfaces defined
- [ ] Props typed correctly
- [ ] Responsive design
- [ ] Accessible (ARIA labels where needed)
- [ ] Performance optimized (useMemo, useCallback)

## Common Tasks

### Adding a New Component
1. Create `.tsx` file in `components/`
2. Define props interface
3. Implement component with hooks
4. Export and import in parent
5. Test in browser

### Modifying Chart Logic
1. Check `types.ts` for data structures
2. Update Recharts configuration
3. Test with `mock-data.json`
4. Verify responsive behavior

### Styling Changes
1. Use TailwindCSS utilities
2. Check mobile responsiveness
3. Maintain consistent spacing/colors
4. Test in different screen sizes

## Git Workflow

### Commit Message Format
Follow Conventional Commits:
```
feat: add new fortune calculation feature
fix: correct K-line chart rendering issue
style: update TailwindCSS classes for better responsiveness
refactor: simplify data processing logic
docs: update README with deployment instructions
```

### Branch Strategy
- `main` - production ready
- `feature/*` - new features
- `fix/*` - bug fixes

## Team Notes

- This is a Chinese astrology visualization app
- K-line charts show life destiny (1-100 years old)
- No backend API - AI generates JSON data
- Support ChatGPT, Claude, Gemini, etc.
- Deployed on Vercel

## Plugin Integration

### Use These Commands
- `/project-starter:architect` - When planning major features
- `/project-starter:commit` - Auto-generate commit messages
- `/project-starter:verify-changes` - Before pushing
- `/project-starter:add-tests` - Generate component tests
- `/project-starter:quick-fix` - Fast lint/type fixes

### Auto-Triggered Agents
- `code-reviewer` - Reviews your changes
- `refactorer` - Suggests improvements
- `docs-writer` - Updates documentation
- `test-architect` - Designs tests
