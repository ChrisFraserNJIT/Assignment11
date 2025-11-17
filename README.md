# Module 8: The Start of the Calculator Webpage Application

# DockerHub URL: https://hub.docker.com/repository/docker/chrisfraser286/601_module8/general

# GitHub URL: https://github.com/ChrisFraserNJIT/Assignment8

Throughout the next few assignments, features and changes will be made to this project will be made utilizing DockerHub and GitHub. These tools will help track the progress of this assignment by showing the changes made and features added.

This README will be updated every time something has been changed or added to this project.


Assignment 11 additions:

For this assignment, I added the new Calculation model using SQLAlchemy with the fields id, a, b, type, and result. I also created the Pydantic schemas CalculationCreate and CalculationRead, including validation to prevent invalid inputs such as division by zero or unsupported calculation types. I reviewed the optional factory pattern and added a simple version to keep the calculation logic organized and easy to extend for future modules.

I also set up and ran the new unit and integration tests for the calculation features. These tests run automatically through the GitHub Actions workflow using a PostgreSQL test container. After all tests passed, the updated Docker image was successfully built and pushed to DockerHub as part of the CI/CD pipeline. The repository now includes updated test files, SQLAlchemy models, Pydantic schemas, and an updated workflow confirming that everything builds and deploys correctly.