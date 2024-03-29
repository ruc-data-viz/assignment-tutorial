# Assignment Tutorial

## Introduction

Here we walk through a short tutorial on starting and completing assignments in this class. We will also go over two intentionally easy practice assignments so you can try out the course tools for yourself.

## Grading

All assignments in this class are GitHub based and graded automatically in GitHub classroom. The grade is based on whether or not the tests pass.

Often, assignments require generating figures which may be different depending on choices you make, many which may be valid. Figures will be graded manually according to the criteria in the assignment.

If you think that an assignment was graded incorrectly due to an error in the automated toolchain, please let me know. This should not happen but if it does it will never be held against you and you will receive proper credit.

## Starting an Assignment

Assignment links will be distributed via email. You can start by clicking the assignment link provided. Authorize GitHub classroom with the permissions it requests and then join the classroom.

You will be prompted to select your student identifier. Find your name on the list and select it. Link your name to your GitHub account there. If you link to the wrong name by accident this can be corrected, but please try to link the correct account!

Once your account is linked, accept the assignment. Wait for the repository to be initialized. This should take a few seconds. Refresh the page to see if the repository is initialized.

When you do this for your first assignment, this will link the account to your identifier in our GitHub classroom. Your account will be automatically linked for all future assignments in this class.

## Completing an Assignment

Assignments are completed by pushing your code to GitHub. There GitHub will run automated tests to grade your assignment. You should run the tests locally (or via a codespace if for some reason you cannot use your local development environment) to make sure they pass before submitting (pushing).

### Running the Tests

Each assignment comes with a `tests.yaml` file which defines the tests that need to run. Run contest with the `tests.yaml` file to check your work. You can do this as many times as you want and you are encouraged to run tests often.

This is meant to simulate a Test Driven Development (TDD) environment. TDD is standard in professional software engineering. You can practice TDD by not writing any code until there is a failing test. Then you may write only the code required to make the test pass. This ensures only the code necessary to make the test pass is written and provides a way to check your work through having to think through program details in designing the test and writing the program. In this class the tests will be written for you.

Run the tests with the following command.

```bash
contest test.yaml
```

### Submitting

You submit your code by committing and pushing to GitHub. You can do this as many times as you like up until the deadline. Remember to use descriptive commit messages to make it easier to see your thought process and to remind your future self what you did on each commit. Remember to commit often so you have many checkpoints to return to.

```bash
git add .
git commit -m "Add my_script.py for task 1"
git push
```

### How GitHub Classroom Grades

GitHub classroom will automatically run the same command you ran (`contest test.yaml`) to test your code. It will check that the output is correct by checking to see if it contains the right strings. Figures and other non-text artifacts generated by your code will be graded manually. The criteria for manual grading will be listed in the assignment. As mentioned above, if you have issues specific to the automatic grading process, please reach out and this will not be held against your grade.