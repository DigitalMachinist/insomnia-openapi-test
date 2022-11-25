# insomnia-openapi-test

This project serves as an example of using Insomnia to produce OpenAPI doc pages via ReDoc and Github actions.

## Documentation

You can view the API docs as rendered by ReDoc here:

[OpenAPI docs live here](https://digitalmachinist.github.io/insomnia-openapi-test/)

## Getting Started with Insomnia

1. [Download and install Insomnia](https://insomnia.rest/download)

2. Click the Create dropdown and import from Git Clone

![Import from Git Clone](images/import-git-clone.png)

3. Authenticate with your Github account

![Authenticate with your Github account](images/auth-github-clone.png)
![Browser authentication success](images/auth-github-success.png)

4. Enter the Github repo URL and click Sync: `https://github.com/DigitalMachinist/insomnia-openapi-test.git` 

![Github repo URL](images/github-clone-url.png)

If everything goes as expected, a new document will be added:

![New document](images/document.png)

5. Click the `games-serving.yaml` document.

6. Click the master branch dropdown and select Branches.

![Branches selection](images/branches.png)

7. Select the API version you plan to implement.

Currently, `v1` is the only API version so checkout `v1`:

![Checkout branch](images/branch-checkout.png)

8. You're all set!

Your Insomnia should be set up and checked out on the correct API version, and you're ready to build your API to the spec.

![You're all set!](images/done.png)

## Running Tests Against Your Implementation

You can use Insomnia to validate your implementation of the API as a self-check.

- Set `base_url` to point to your API server.

- Open the `Debug` tab to call API routes with custom JSON payloads for one-off tests of routes as you work.

- Open the `Test` tab to execute our full test suite against your API implementation to validate that all your routes meet our spec.