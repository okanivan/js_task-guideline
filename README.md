# Guideline how to implement solution for JS tasks

Every task:
- Includes `eslint`
- Includes `pre-commit` hooks (eslint)
- Includes `ci` (travis-ci) 

## Requirements

- `NodeJS`, `npm` [download](https://nodejs.org/en/) or [read installation guide](https://nodejs.org/en/download/package-manager/)
- `git` [download](https://git-scm.com/downloads) or [read installation guide](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

## Learn before writing solution

- [Creating a pull request from a fork](https://help.github.com/en/articles/creating-a-pull-request-from-a-fork)

## Workflow

- Fork the repository with task
- Clone forked repository<br/> `git clone git@github.com:<user_name>>/<task_repository>.git`
- Create separate branch for the solution. Name of the branch should be the same as name of your channel in slack. <br/> e.g. `git checkout -b fs_on_apr19_sasha`
- Run `npm install` to install dependencies
- Implement the solution inside function scope in `src/<task_name>.js`
- Make sure the code is clean. Run eslint (`npm run lint`)
- Make sure the solution works. Run tests (`npm run test`)
- Push code to the repository in created branch<br/> `git push origin <branch_name>`
- Create `Pull Request` from forked repo (`<branch_name>`) to original repo (`master`)
- Add your coach / TA to reviewers and send them a link of created `PR`

## Scripts
- `npm run test` - run tests specified in `<task_name>.test.js`
- `npm run lint` - run eslint