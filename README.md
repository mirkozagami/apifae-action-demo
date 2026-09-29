# apifae-action-demo

A working example of [apifae/action](https://github.com/apifae/action): it checks a live API against an APIFae workspace on every push and pull request.

- `main` serves an API that matches the mocks, so the check is green.
- [Pull request #1](https://github.com/mirkozagami/apifae-action-demo/pull/1) changes the API so `count` becomes a string, and the check goes red on the drift.

The "API" is a plain HTTP server over `api/`, started inside the workflow. The workflow uses the action's five-line setup with only the URL changed.
