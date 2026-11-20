14. Cross-questions / Viva questions with answers
These are important questions that your teacher can ask after the practical.
Basic questions
Q1. What is GitHub Actions?

GitHub Actions is an automation platform provided by GitHub that helps automate software development tasks such as building, testing, and deploying applications.

Q2. What is the main purpose of GitHub Actions?

Its main purpose is to automate repetitive development tasks and implement CI/CD pipelines.

Q3. What is CI?

CI stands for Continuous Integration. It is a software development practice in which developers frequently integrate their code changes into a shared repository and automatically build and test them.

Q4. What is CD?

CD stands for Continuous Delivery or Continuous Deployment. It automates the process of preparing or releasing software.

Q5. Is GitHub Actions a CI/CD tool?

Yes. GitHub Actions supports both Continuous Integration and Continuous Delivery/Deployment.

Q6. Do we need to install GitHub Actions on our computer?

No. GitHub Actions is integrated into GitHub. We configure workflows in our repository, and GitHub executes them using runners.
Technical questions
Q7. What is a workflow?

A workflow is an automated process defined in a YAML file that contains jobs and steps.

Q8. Where are workflow files stored?

Inside the .github/workflows/ directory of the repository.

Q9. What is the extension of a workflow file?

.yml or .yaml.

Q10. What is a runner?

A runner is a machine that executes the jobs and steps defined in a GitHub Actions workflow.

Q11. What is ubuntu-latest?

It specifies that our workflow should execute on a GitHub-hosted Ubuntu Linux runner.

Q12. What is the difference between uses and run?
- uses executes a reusable action.
- run executes shell commands directly on the runner.
Q13. What is actions/checkout?

It is an action that checks out the repository code so that the runner can access the project files.

Q14. What is actions/setup-java?

It is an action that installs and configures the required Java version on the runner.

Q15. What is the purpose of on in YAML?

It defines the events that trigger the workflow.

Q16. What happens when a test fails?

The corresponding step fails, and the workflow run is marked as failed unless failure handling has been specially configured.
Practical-based questions
Q17. Which programming language did you use in this experiment?

Java.

Q18. Which Java version did you configure?

Java 21.

Q19. Which operating system did you use for the runner?

Ubuntu Linux.

Q20. Which events did you configure?

Push and pull request events targeting the main branch.

Q21. Why did you create CalculatorTest.java?

To verify whether the addition method produces the expected result.

Q22. What is the difference between Git and GitHub?

Git is a distributed version control system, whereas GitHub is a cloud-based platform for hosting Git repositories and collaborating on projects.

Q23. What is the difference between Jenkins and GitHub Actions?
Jenkins	GitHub Actions
Automation server	GitHub-integrated automation platform
Usually requires separate setup	Workflows configured inside GitHub
Uses Jenkinsfile (commonly Groovy)	Uses YAML
Supports plugins	Supports reusable actions

Q24. Can GitHub Actions work with Docker?

Yes. It can build Docker images, run containers, test applications inside containers, and automate deployment.

Q25. What happens if you push code three times?

If all three pushes trigger the configured workflow, GitHub creates a workflow run for each push. The runs may execute independently or concurrently, subject to workflow configuration and available runner capacity.

15. Quick revision – Check your understanding
Try answering these five questions without looking at the explanations above.
Viva practice
0/5 answered

Q1. Where should a GitHub Actions workflow file be stored?

src/

test/

.github/workflows/

bin/



Q2. What is the purpose of a runner?

Store Java files

Execute workflow jobs

Create GitHub accounts

Write YAML files



Q3. Which keyword executes shell commands?

uses

with

run

on



Q4. What triggers our pipeline?

Only opening VS Code

Push and pull_request

Installing Java

Creating a folder



Q5. What happens if our test case fails?

Workflow always succeeds

GitHub deletes the repository

The workflow is marked failed

Java is uninstalled


Submit answers
16. Official documentation
For additional reference:
- GitHub Docs – Building and Testing Java with Maven
- GitHub Docs – Writing Workflows
- GitHub Actions – Setup Java
One important thing to remember: In this experiment, your laptop writes and pushes the code, GitHub stores the code, and the GitHub Actions runner automatically builds and tests it. That's the complete concept of your practical.
