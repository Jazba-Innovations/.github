## Commit Formats for Better Collaboration

Making meaningful commits is is essential for better collaboration and maintaining a clear history of changes, otherwise PRs won't be accepted. Follow the guidelines below for writing meaningful commit messages:

<br />

1. **Include Affected Area:** _Mention the folder or page that the changes belong to in the commit message. This provides context about which part of the project is being modified._

2. **Use Conventional Commits:** _Conventional commits follow a structured format, which makes it easier to understand the changes and automate processes like generating changelogs. The format is: `<type>(<scope>): <description>`_

     - `<type>:` Represents the type of the commit (e.g., feat, fix, chore, docs, style, etc.)
     - `<scope>:`  Denotes the affected module, component, or area of the project.
     - `<description>:` A concise description of the changes.
  
3. **Be Specific:** _Clearly describe the purpose of the changes. Avoid vague or generic statements._

4. **Use Imperative Tense:** _Write commit messages in the imperative mood (e.g., "update," "fix," "add," instead of "updated," "fixed," "added")._

<br />
<hr />
<br />

### Commit Types:

Here are some common commit types. Learn more about it [in this article](https://medium.com/@simongideon918/upscaling-your-github-commit-messages-d360f94843e4)

- `feat`: Use when introducing a new feature.
- `fix`: Apply when fixing a bug or issue.
- `docs`: Use for documentation updates.
- `style`: Apply when making code formatting or style changes.
- `refactor`: Use when performing code refactoring without introducing new features or bug fixes.
- `test`: Apply when adding or updating tests.
- `chore`: Use for maintenance tasks, build-related changes, etc.


<br />

Here is an example of a valid / invalid commit:


```
# BAD COMMIT MESSAGE
$ git commit -m 'fixed some issues'

# GOOD COMMIT MESSAGE
$ git commit -m 'feat(user-profile): implement user bio editing feature'


# BAD COMMIT MESSAGE
$ git commit -m 'added new feature'

# GOOD COMMIT MESSAGE
$ git commit -m 'fix(authentication): resolve login redirection bug'


# BAD COMMIT MESSAGE
$ git commit -m 'update readme'

# GOOD COMMIT MESSAGE
$ git commit -m 'docs(readme): update installation instructions'


# BAD COMMIT MESSAGE
$ git commit -m 'update styling'

# GOOD COMMIT MESSAGE
$ git commit -m 'style(login-form): format code according to the style guide'


# BAD COMMIT MESSAGE
$ git commit -m 'create new compnent for user service'

# GOOD COMMIT MESSAGE
$ git commit -m 'refactor(user-service): extract user validation logic into a separate function'


# BAD COMMIT MESSAGE
$ git commit -m 'add tests'

# GOOD COMMIT MESSAGE
$ git commit -m 'test(user-service): add unit tests for user authentication'



# BAD COMMIT MESSAGE
$ git commit -m 'update deploymeny'

# GOOD COMMIT MESSAGE
$ git commit -m 'chore(deploy): update deployment script for automatic CI/CD'

```