# ESLint Usage Guide

This project now includes ESLint configuration for JavaScript code quality and consistency.

## Rules Configured

1. **semi** (error): Enforces semicolons at the end of statements
   - All JavaScript statements must end with a semicolon
   - This prevents automatic semicolon insertion issues

2. **no-unused-vars** (warning): Warns about unused variables
   - Helps identify dead code and potential bugs
   - Variables declared but never used will trigger a warning

## Usage

### Check for linting issues:
```bash
npm run lint
```

### Auto-fix issues (including missing semicolons):
```bash
npm run lint:fix
```

### Manual ESLint commands:
```bash
# Lint a specific file
npx eslint path/to/file.js

# Lint and fix a specific file
npx eslint path/to/file.js --fix

# Lint all JavaScript files
npx eslint '**/*.js'
```

## Installation

If node_modules is not present, install dependencies:
```bash
npm install
```

## Configuration Files

- `.eslintrc.json` - ESLint configuration with rules
- `package.json` - Project dependencies and npm scripts
