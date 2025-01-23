## 🚀 How to Use Conventional Commits in Your Git Workflow

Conventional Commits standardize your commit messages, making your project history clear and consistent. Follow this guide to integrate them into your workflow.

---

### 1. **Commit Messages Using `git commit` in the Terminal**

To commit changes, you'll use the `git commit` command while adhering to the Conventional Commit format.

#### Example Command:

```bash
git commit -m "feat(auth): add Google login feature"
```

---

### 2. **Steps to Commit in the Terminal**

1. **Make Changes**: Modify your files as needed.

2. **Stage Your Changes**: Add the modified files to the staging area:

   - To add a specific file:
     ```bash
     git add <file>
     ```
   - To add all changed files:
     ```bash
     git add .
     ```

3. **Commit with Conventional Commit Message**:

   ```bash
   git commit -m "feat(button): add rounded corners"
   ```

4. **Push the Changes**: Push your commits to the remote repository:
   ```bash
   git push
   ```
   Or, to push to a specific branch:
   ```bash
   git push origin <branch-name>
   ```

---

### 3. **Conventional Commit Structure**

Each commit message follows this structure:

```
<type>(<scope>): <description>
```

#### Components:

- **`type`**: The kind of change (e.g., `feat`, `fix`, `chore`).
- **`scope`** (optional): The specific area of the project affected (e.g., `auth`, `frontend`).
- **`description`**: A concise explanation of the change.

---

### 4. **Commit Types**

| **Type**     | **Description**                                            | **Example**                                 |
| ------------ | ---------------------------------------------------------- | ------------------------------------------- |
| **feat**     | A new feature for the user or system                       | `feat(auth): add Google login feature`      |
| **fix**      | A bug fix for the user or system                           | `fix(button): resolve button hover issue`   |
| **chore**    | Routine tasks like maintenance or dependency updates       | `chore(deps): update react to v17.0.2`      |
| **docs**     | Documentation updates                                      | `docs(readme): update installation guide`   |
| **style**    | Code style changes (e.g., formatting, missing semi-colons) | `style(css): fix button alignment`          |
| **refactor** | Code changes that don't fix bugs or add features           | `refactor(auth): simplify login validation` |
| **test**     | Adding or updating tests                                   | `test(auth): add unit tests for login`      |
| **build**    | Build system or dependency changes                         | `build(webpack): add production config`     |
| **ci**       | Continuous integration-related changes                     | `ci(gitlab): update deployment pipeline`    |
| **perf**     | Performance improvements                                   | `perf(api): optimize database queries`      |
| **env**      | Environment setup or configuration changes                 | `env(docker): update staging Dockerfile`    |
| **sec**      | Security improvements                                      | `sec(auth): encrypt user passwords`         |
| **config**   | Configuration file updates                                 | `config: update .eslint rules`              |
| **api**      | Updates to API contracts or integrations                   | `api(user): add profile update endpoint`    |

---

### 5. **Additional Commit Types**

| **Type**   | **Description**             | **Example**                                   |
| ---------- | --------------------------- | --------------------------------------------- |
| **revert** | Reverts a previous commit   | `revert(auth): rollback Google login feature` |
| **merge**  | Indicates a merge commit    | `merge: branch 'feature/auth' into 'main'`    |
| **deps**   | Dependency-specific updates | `deps: bump axios from 0.21.1 to 0.24.0`      |
| **design** | UI or UX improvements       | `design(button): update hover effect`         |

---

[Conventional Commits Specification](https://www.conventionalcommits.org).

---
