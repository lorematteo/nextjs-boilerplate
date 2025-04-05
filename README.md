# ⚛️ Next.js Boilerplate

## 🚀 Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

## ⚙️ Available Scripts

- `dev`: Start development server
- `build`: Build for production
- `start`: Start production server
- `lint`: Run ESLint with zero tolerance for warnings
- `format`: Check formatting with Prettier
- `format:fix`: Fix formatting issues
- `typecheck`: Run TypeScript type checking
- `validate`: Runs code quality checks (typecheck, lint, format) in parallel to ensure your code meets project standards
- `validate-and-build`: Run checks and build
- `deploy`: Validate, build and start

## 🛡️ Code Quality

The `validate` script is a comprehensive code quality check that:
- Verifies type safety with TypeScript
- Ensures code follows ESLint rules with zero warnings allowed
- Confirms all files adhere to Prettier formatting standards

This script runs automatically as a pre-commit hook via Husky to maintain consistent code quality throughout development.

## 💬 Commit Guidelines

This project uses commitlint to enforce consistent commit messages. When committing changes:

1. Format your commit message as: `type(scope): subject`

2. Valid types include:
   - `feat`: New features
   - `fix`: Bug fixes
   - `docs`: Documentation changes
   - `style`: Code style changes (formatting, etc.)
   - `refactor`: Code changes that neither fix bugs nor add features
   - `test`: Adding or modifying tests
   - `chore`: Changes to the build process or auxiliary tools
   - `evol`: Evolution of existing functionality
   - `ci`: Changes to CI configuration files and scripts
   - `revert`: Reverting a previous commit
   - `build`: Changes that affect the build system

3. Example commit messages:
   ```
   feat(auth): add login component
   fix(navbar): resolve dropdown positioning issue
   docs(readme): update installation instructions
   ```

4. Pre-commit hooks will automatically:
   - Run the validate script to check code quality
   - Verify your commit message format

## 🏗️ Project Structure

This project follows the Next.js App Router architecture with TypeScript and has integrated:

- ESLint for code quality
- Prettier for code formatting
- TypeScript for type checking
- Tailwind CSS for styling
- Husky for Git hooks
- Commitlint for commit message validation
