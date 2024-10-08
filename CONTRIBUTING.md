# Contributing Guidelines

Thank you for taking the time to contribute to our project. Please read the following guidelines to propel your contribution:

- The project is developed using a monorepo structure with yarn workspaces and Nx.
- It is comprised of the following packages:
  - common (Shared code like loggers, utils, middlewares, etc.)
  - core (Shared code like configurations, constants, dependency injection etc.)
  - data (Shared code like database configuration, caching confiuration etc.)
  - recall-api (Express Server)
  - eslint-config (Shared ESLint configuration)
  - jest-config (Shared Jest configuration)

### Recall API
- This is the main package that contains the Express server.
- To add a module, create a new folder in the `packages/recall-api/src/modules/` directory.
- You can copy the `packages/recall-api/src/modules/example/` folder and rename it to your module name.


> **⚠️IMPORTANT**
>
> **Pull Requests _having no issue associated_ with them _will not be accepted_. Firstly get an issue assigned, whether it's already opened or raised by you, and then create a Pull Request.**
>
> **An automated process is in the process of implementation to ensure the timely management of Pull Requests (PRs) on this platform.**
>
> **PRs that have been open for a duration exceeding 45 days will be automatically closed, so please plan accordingly.**

## How to Contribute 🤔

To get started, look at the existing [**Issues**](https://github.com/Friendsofthepeople/recall-server/issues) or [**create a new issue**](https://github.com/Friendsofthepeople/recall-server/issues/new/choose)!

## Issues 🎃

- Select an issue template from the [issues](https://github.com/Friendsofthepeople/recall-server/issues) tab. Otherwise, choose **Other** if it doesn't match what you're looking for.
- When creating an issue, make sure you fill up all the fields properly.
- Make sure that you are NOT raising a **duplicate issue**.
- If you want to work on the issue, please click on the _I am willing to work on this issue_ checkmark.
- **Note:** If you aren't the owner of the issue, please comment that you're willing to work on the issue and wait for maintainers to assign you the issue. Also, don't work on the issue if you're NOT assigned.
- Please do **not** start working on the issue if you aren't yet assigned and have the `ready 🚀` label.
- Work on only **ONE** issue at a time.

**Closing the issue** 📍

- If you decide to close the issue, please leave a brief comment describing why(e.g., I'm busy with other obligations.) before you do.
- **Note:** If the Pull Request associated with the issue gets merged and the issue still remains open, it's **your** responsibility to close the issue.

## Commits Message Guidelines 💬

We follow a standardized commit message format using Commitlint to ensure consistency and clarity in our commit history. Each commit message should adhere to the following guidelines:

1. **Type**: The commit type must be one of the following:

   - `feat`: A new feature or enhancement.
   - `fix`: A bug fix.
   - `docs`: Documentation changes.
   - `style`: Code style changes (e.g., formatting, semicolons).
   - `refactor`: Code refactorings with no feature changes or bug fixes.
   - `test`: Adding or improving tests.
   - `chore`: General maintenance tasks, build changes, etc.

2. **Scope** (Optional): The scope provides context for the commit, indicating the specific part of the project being affected. Use a short description in lowercase (e.g., `auth`, `navbar`, `README`).

3. **Description**: A brief and meaningful description of the changes made. Start with a capital letter and use the imperative mood (e.g., "Add new feature" instead of "Added new feature").

4. **Issue reference** (Optional): Include the issue number associated with the commit (e.g., `#123`).

#### ✔️ Examples of Valid Commit Messages

- `feat: Add user authentication feature`
- `fix(auth): Resolve login page redirect issue`
- `docs: Update installation instructions`
- `style: Format code according to project guidelines`
- `refactor(navbar): Improve responsiveness`
- `test: Add unit tests for API endpoints`
- `chore: Update dependencies to latest versions`
- `fix: Handle edge case in data processing (#456)`

#### ❌ Examples of Invalid Commit Messages

- `Added new stuff`
- `Fixed a bug`
- `Updated code`
- `auth feature update`
- `chore: fixed some stuff`

### Commit Example with Commitlint

```bash
git commit -m "feat(auth): Implement user signup process (#789)"
```

---

## 🔁 Making Pull Requests

1. When you submit a pull request, several tests will automatically be run
   as GitHub Actions. If any of these tests fail, it is your responsibility to try and resolve the underlying issue(s). If you don't know how to resolve the underlying issue(s), you can ask for help.

2. Each pull request should contain a single logical change or related set of changes that make sense to submit together. If a pull request becomes too large or contains too many unrelated changes, it becomes too difficult to review. In such cases, the reviewer has the right to close your pull request and ask that you submit a separate pull request for each logical set of changes that belong together.

3. Link the issue you have resolved in the Pull Request Template (e.g. Closes/Fixes #99).
4. Use our [Commit messages Guidelines](https://github.com/Friendsofthepeople/recall-server/main/CONTRIBUTING.md#commits-message-guidelines-) for your changes.
5. Do not re-open a pull request that a reviewer has closed.
   - Make sure to tick the "Allow edits from maintainers" box. This allows us to directly make minor edits / refactors and saves a lot of time.
     > **Note**
     > If your pull request has merge conflicts with the `main` branch (GitHub checks for this automatically and notifies you), you are responsible for resolving them. You can do this by merging the `main` branch into your branch (`git pull upstream main`), and then pushing the updated branch to your fork (`git push`). If you need more tips, check out [Resolving a merge conflict on GitHub](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-on-github).

---

## Remarks ✅

- If something is missing here, or you feel something is not well described, either create a PR, [raise an issue](https://github.com/Friendsofthepeople/recall-server/issues), or [do a code review of the person’s PR](https://www.freecodecamp.org/news/code-review-tips/) (ensure that your review conforms to the [Code of Conduct](https://github.com/Friendsofthepeople/recall-server/CODE_OF_CONDUCT.md))

- You can tag maintainers for any kind of difficulty using `@username`.

### Levels

We came up with this chart so you can gauge the issue's difficulty and pick ones that fit within your skillset:
| Points              | Contribution                                                                |
|---------------------|-----------------------------------------------------------------------------|
| `priority: low`:    | Addition of new links/categories or doing any small task (e.g fixing typos) |
| `priority: medium`: | Modifying an existing feature                                               |
| `priority: high`:   | Making completely new feature                                               |

## 🙏 Thanks to all Contributors
Thanks a lot for spending your time in helping Recall Server grow. Thanks a lot! ❤️
 <a href = "https://github.com/Friendsofthepeople/recall-server/graphs/contributors"> <br />
   <img src="https://contrib.rocks/image?repo=Friendsofthepeople/recall-server" />
 </a>