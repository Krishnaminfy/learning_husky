# learning_husky

# Git Hooks & CI Automation – Learning Project

This project is part of my learning assignment focused on improving code quality and workflow automation using Git tools. It was my first time working with tools like **Husky**, **lint-staged**, and **GitHub Actions**, and this README documents what I’ve learned so far.

---

##  What is Husky?

Before this assignment, I had never used **Husky**, but I’ve now learned what it does and why it’s useful.

Husky helps add **Git hooks** — little scripts that run before certain Git commands, like committing or pushing code. With Husky, you can automatically check for code issues before they get committed. For example:

- Run a linter before every commit
- Format code automatically
- Block bad commit messages
- Prevent broken code from being pushed

Basically, Husky adds automation to your Git workflow to **catch mistakes early** and **keep code clean**.

---

##  What I Set Up

### 1. **Husky + lint-staged**
- Installed Husky and lint-staged to run checks before committing code.
- Hook runs automatically when I try to commit, ensuring code quality.

### 2. **Pre-commit Hook**
- Runs **ESLint** and **Prettier** on staged files.
- If code isn’t formatted or has lint errors, the commit is rejected until it's fixed.

### 3. **Commit Message Validation**
- Using **commitlint**, I set up rules for how commit messages should look (like `feat:`, `fix:`, etc.).
- Invalid commit messages get blocked automatically.

### 4. **GitHub Actions CI**
- Set up a GitHub Actions workflow that runs on every push or pull request.
- It installs dependencies and runs ESLint as part of a basic CI pipeline.

---

##  What I Tried

I tested the setup by trying to:
- Commit code with lint errors —  Rejected
- Use a bad commit message —  Rejected
- Push clean code with a proper message —  Accepted

This helped me understand how automation can stop mistakes before they become problems.

---

##  What I Learned

Even though this was my first time using these tools, I realized how powerful they are for real-world development.

### Why This Matters:
- Saves time by catching problems early
- Enforces consistent code formatting
- Encourages writing meaningful commit messages
- Makes collaborating in teams much smoother

Automation like this doesn’t replace good practices — it reinforces them.

---

##  Tools Used

- **Husky** – for Git hooks
- **lint-staged** – to run checks on staged files
- **ESLint** – for JavaScript code linting
- **Prettier** – for consistent code formatting
- **commitlint** – for commit message rules
- **GitHub Actions** – for CI on push/pull

---

##  What’s Next?

Now that I understand the basics, I’d like to explore more automation — like running unit tests, checking code coverage, or even deploying code automatically through CI/CD.

---
