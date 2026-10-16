# Developer Learning Notes

**Date:** 15 October 2026  
**Session type:** Technical knowledge sharing  
**Presenters:** Me and my friend

These notes cover UI/UX Design, Software Architecture, AI Engineering, QA Engineering, and a DevOps Engineer beginner guide. They summarize the main concepts, responsibilities, tools, examples, and career paths discussed.

---

## 1. UI/UX Designer

### 1.1 Introduction

A UI/UX designer helps create websites, mobile applications, and other digital products that are attractive and easy to use. The main goal is to provide a useful, clear, and positive experience for users.

### 1.2 What is UI/UX design?

- **UI (User Interface):** Focuses on the visual appearance of a website or application, including colours, buttons, fonts, icons, and layouts.
- **UX (User Experience):** Focuses on how users interact with a product and how easily they can complete their tasks.

UI and UX work together to make digital products both visually clear and user-friendly.

### 1.3 Responsibilities of a UI/UX designer

- Understand users' needs and expectations.
- Design website and mobile application interfaces.
- Create wireframes and prototypes before development.
- Test designs to identify usability problems.
- Improve designs based on user feedback.
- Collaborate with developers to build the final product.

### 1.4 Skills and tools

**Important skills**

- Creativity and visual design
- Communication and teamwork
- Problem-solving
- User research
- Understanding user behaviour

**Common tools**

- **Figma:** Interface design and prototyping
- **FigJam:** Brainstorming and user flows
- **Canva:** Creating visual designs
- **Adobe XD:** Interface design and prototyping

### 1.5 Real-world example

Consider an online shopping application. A UI/UX designer helps users easily search for products, view product details, add items to a shopping cart, and complete purchases. The designer organizes the interface clearly and tests whether users can complete these tasks without confusion.

### 1.6 Career opportunities

- **UI Designer:** Designs the visual appearance of interfaces.
- **UX Designer:** Improves usability and the overall user experience.
- **Product Designer:** Designs the overall experience of a digital product.
- **UX Researcher:** Studies user needs, behaviour, and feedback.
- **Interaction Designer:** Designs how users interact with interface elements.

### 1.7 Conclusion

UI/UX design is an important part of software development. Good design helps users understand and use digital products easily. A successful UI/UX designer combines creativity, user research, and problem-solving to create useful and accessible experiences.

---

## 2. Software Architecture

### 2.1 What is software architecture?

Software architecture is the high-level structure of a software system. It defines the main components of the system and how they communicate with each other.

**Simple example:** Building a house requires a plan before construction. Similarly, software needs a plan that explains how the frontend, backend, database, and other components work together.

### 2.2 Why do we need software architecture?

1. **Planning:** Helps developers plan how to build the software.
2. **Maintainability:** Makes the system easier to update and fix.
3. **Scalability:** Helps the system handle growth in users and workload.
4. **Security:** Helps developers plan how to protect user data.
5. **Performance:** Supports efficient use of system resources.
6. **Teamwork:** Helps developers understand components and responsibilities.

### 2.3 Main components of a typical web application

#### Frontend

The frontend is the part of an application that users can see and interact with.

**Technologies:** HTML, CSS, JavaScript, Bootstrap.

**Examples:** Login pages, buttons, forms, and the home page.

#### Backend

The backend handles application logic and processes requests from users or other systems.

**Technologies:** PHP, Laravel, Python, Java.

**Examples:** Checking login details, processing book requests, and validating user information.

#### Database

The database stores and manages application data.

**Technologies:** MySQL, PostgreSQL, MongoDB.

**Examples:** Storing user details, book information, exchange requests, and reviews.

### 2.4 How do these components work together?

For example, when a user logs in:

1. The user enters a username and password on the frontend.
2. The frontend sends the login request to the backend.
3. The backend validates the submitted information.
4. The backend queries the database for the required user information.
5. The backend returns a response to the frontend.
6. The frontend displays the result to the user.

This is a basic request-and-response workflow in a web application.

### 2.5 Types and styles of software architecture

#### A. Monolithic architecture

In monolithic architecture, the main application functions are combined into one application.

**Example:** Login, book management, exchange requests, and administration are handled within one Laravel application.

**Advantages**

- Easy to develop for small projects.
- Usually straightforward to deploy.
- Simple to manage initially.

**Disadvantages**

- Can become difficult to maintain as the application grows.
- Tightly coupled code can make changes in one area affect others.

#### B. Layered architecture

Layered architecture divides an application into layers with different responsibilities.

- **Presentation layer:** Displays the user interface.
- **Business logic layer:** Handles application rules.
- **Data access layer:** Communicates with the database.

**Example:** A Laravel application that separates request handling, business logic, and database operations.

**Advantages**

- Organizes code clearly.
- Supports maintenance and testing.
- Gives each layer a defined responsibility.

#### C. Microservices architecture

Microservices architecture divides a larger application into smaller, independently deployable services that communicate through defined interfaces or APIs.

**Example services**

- User Service
- Book Service
- Notification Service

**Advantages**

- Services can be developed and deployed independently.
- Individual services can scale separately.

**Disadvantages**

- More difficult to develop and operate.
- Requires additional service communication, deployment, and monitoring.

#### D. Client–server architecture

In client–server architecture, a client sends requests to a server, and the server processes the requests and returns responses.

- **Client:** A web browser or mobile application.
- **Server:** Processes requests and provides responses.

**Example:** A browser requests a website page from a web server.

**Advantages**

- Centralizes data and processing.
- Allows multiple clients to use shared server resources.

#### E. Event-driven architecture

In event-driven architecture, an event triggers one or more actions. Components can react to events without every component needing to perform all work directly.

**Example:** When a student submits a book exchange request, the system generates an event that triggers a notification to the book owner.

**Advantages**

- Useful for notifications and asynchronous tasks.
- Allows components to respond to events independently.

#### F. MVC (Model–View–Controller)

MVC separates an application's responsibilities into three parts:

- **Model:** Represents and manages data and related rules.
- **View:** Presents the user interface.
- **Controller:** Receives requests and coordinates the required actions.

**Example in Laravel:** Models work with data, Blade views render pages, and controllers handle requests and coordinate application logic.

**Advantages**

- Organizes code into clear responsibilities.
- Supports easier development and maintenance.
- Separates presentation from other application concerns.

**Important note:** MVC is a design pattern or architectural pattern commonly used within a broader application architecture. It is not necessarily an alternative to monolithic, layered, or microservices architecture; these concepts can be combined.

---

## 3. AI Engineering

### 3.1 What is AI engineering?

AI engineering focuses on building, deploying, and maintaining production-ready software products that use AI models.

The work involves turning a model or AI capability into a reliable, secure, scalable, and cost-effective product.

A useful distinction:

- **Data science:** Uses data to discover insights and answer questions.
- **Machine learning engineering:** Builds, trains, evaluates, and operationalizes machine-learning models.
- **AI engineering:** Builds the wider product and system around AI capabilities.

These roles overlap, and their responsibilities vary by organization.

### 3.2 AI engineering lifecycle

#### Phase 1: Data engineering

- **Data collection:** Gather data from databases, APIs, PDFs, and websites where permitted.
- **Data cleaning:** Remove duplicates and handle missing or inconsistent values.
- **Data validation:** Check data quality, relevance, and potential bias.

**Tools:** Python, Pandas, SQL, Apache Spark.

#### Phase 2: Model selection and development

- Select an appropriate model for the task, such as a large language model (LLM) for text, a diffusion model for image generation, or a computer-vision model for object detection.
- Train, fine-tune, or use transfer learning when appropriate.
- Evaluate performance using suitable metrics, such as accuracy, precision, recall, and F1-score for relevant classification tasks.

**Tools:** PyTorch, TensorFlow, Hugging Face Transformers.

#### Phase 3: Core AI engineering

**A. Retrieval-Augmented Generation (RAG)**

RAG connects an AI model to relevant external information, such as organizational documents. The system retrieves useful information and supplies it as context for generating an answer, often without retraining the model.

**Example:** A chatbot that answers questions using approved government-department documents.

**B. Prompt engineering**

Prompt engineering involves designing instructions and examples to help a model produce useful, consistent outputs. Techniques include system instructions and few-shot prompting.

**C. Vector databases and embeddings**

Embeddings represent text or other data as numerical vectors. A vector database stores and searches these representations to find semantically similar content.

**Examples:** Chroma, Pinecone, Qdrant, Weaviate.

**D. Orchestration**

Orchestration coordinates multiple AI-related steps, such as retrieval, model calls, tool use, and output processing.

**Examples:** LangChain, LlamaIndex.

**E. AI agents**

An AI agent can use available tools, such as search, calculators, or APIs, to perform steps toward a goal. The tools and permissions it receives should be carefully controlled.

#### Phase 4: Application and system architecture

- **Build an API:** Expose model functionality through an API, for example with FastAPI or Flask.
- **Design the system:** Plan how the frontend, backend, AI model, and database communicate.
- **Optimize performance:** Reduce latency and cost using suitable techniques such as caching, batching, and model quantization.

#### Phase 5: MLOps and LLMOps

MLOps and LLMOps cover the deployment, operation, monitoring, and improvement of machine-learning and language-model systems.

- **Containerization:** Package applications using tools such as Docker.
- **Deployment:** Deploy to an appropriate cloud or server environment.
- **CI/CD:** Automate testing and deployment with tools such as GitHub Actions.
- **Monitoring:** Track latency, errors, costs, model quality, and user feedback.

**Examples of platforms and tools:** AWS, Google Cloud, Azure, LangSmith, Weights & Biases.

#### Phase 6: Safety and evaluation

- **Guardrails:** Reduce risks such as unsafe outputs, prompt injection, and inappropriate tool use.
- **Evaluation:** Test answer quality, factual grounding, retrieval quality, and task success. RAGAS is one example of a RAG evaluation framework.
- **Privacy and fairness:** Protect sensitive data and assess potential bias.
- **Ongoing monitoring:** Re-evaluate the system when data, models, prompts, or user needs change.

No single technique can eliminate hallucinations or guarantee safety, so layered controls and continuous evaluation are important.

### 3.3 AI engineer skill stack

**Fundamentals**

- Python
- SQL
- Git
- REST APIs
- Linux basics

**AI foundations**

- Machine learning basics
- Deep learning
- Natural language processing
- Embeddings
- Transformer architecture

**Engineering tools**

- Backend development: FastAPI and Python
- Vector databases: Chroma or a hosted alternative
- AI frameworks: LangChain or LlamaIndex
- Model integration: relevant model APIs and SDKs
- Cloud platforms: AWS or Google Cloud
- DevOps: Docker and basic Kubernetes knowledge

### 3.4 AI engineer vs. ML engineer vs. data scientist

| Role | Main question | Typical output |
|---|---|---|
| Data Scientist | What does the data tell us? | Insights, experiments, and analytical reports |
| ML Engineer | How can we build and operate a useful model? | Trained and deployed model |
| AI Engineer | How can we build a useful product using AI? | An integrated AI application, assistant, or service |

These are general distinctions rather than strict boundaries; many teams combine responsibilities.

### 3.5 Three-month beginner roadmap

#### Month 1: Python and AI basics

- Learn Python, APIs, and basic software development.
- Understand how large language models work at a high level.
- Build small applications that use an AI API.

#### Month 2: RAG

- Build a chatbot that answers questions about your own PDF documents.
- Learn document processing, embeddings, retrieval, and a vector database.
- Evaluate whether answers are supported by the source documents.

#### Month 3: Deployment

- Package the application with Docker.
- Deploy it to an appropriate hosting environment.
- Add error handling, logging, monitoring, and basic security controls.

**Suggested portfolio projects**

1. A RAG chatbot using a custom document collection, such as public government information.
2. An AI agent that uses approved tools to search information and perform bounded tasks.
3. An end-to-end AI product with an API, user interface, deployment, and monitoring.

Three months is a starting plan, not a guarantee of job readiness. Progress depends on prior experience and the time available for practice.

---

## 4. QA Engineer (Quality Assurance Engineer)

### 4.1 Overview

A QA Engineer helps ensure software works correctly, reliably, and according to requirements. QA work aims to prevent defects, identify problems early, and provide evidence about product quality before release.

### 4.2 Main responsibilities

- Understand requirements and user stories.
- Write test plans and test cases.
- Perform manual and automated tests.
- Report and track defects.
- Retest fixes.
- Perform regression testing to check that existing features still work.
- Help assess whether the product is ready for release.

### 4.3 Typical QA process

1. **Requirement analysis:** Read specifications and identify missing, unclear, or conflicting requirements.
2. **Test planning:** Define the scope, tools, schedule, resources, and risks.
3. **Test case design:** Document steps, test data, and expected results.
4. **Environment setup:** Prepare the test server, data, devices, and configurations.
5. **Test execution:** Run tests and record actual results.
6. **Defect reporting:** Record issues with reproduction steps, evidence, and severity.
7. **Retesting and regression testing:** Confirm fixes and check for unintended side effects.
8. **Test closure:** Summarize results, remaining risks, and relevant release information.

The exact process varies depending on the team and development method.

### 4.4 Types of testing

- **Functional testing:** Checks whether features behave according to requirements.
- **Regression testing:** Checks that changes have not broken existing features.
- **Integration testing:** Checks interactions between components.
- **System testing:** Tests the complete system.
- **User Acceptance Testing (UAT):** Supports confirmation that the product meets business needs.
- **API testing:** Checks API responses, validation, errors, and behavior.
- **Performance and load testing:** Evaluates responsiveness and behavior under workload.
- **Security testing:** Identifies security weaknesses.
- **Usability testing:** Checks how easily users can complete tasks.
- **Compatibility testing:** Checks behavior across supported browsers, devices, and environments.

### 4.5 Responsibilities in practice

**Planning**

- Create test strategies and test plans.
- Estimate testing effort and identify risks.

**Execution**

- Perform manual testing.
- Write automation scripts when appropriate.
- Maintain automated test suites.

**Reporting**

- Log defects clearly in tools such as Jira.
- Share test results and metrics, such as pass/fail counts and defect trends.

**Collaboration**

- Work with developers to reproduce and resolve bugs.
- Work with product owners and business analysts to clarify requirements.
- Participate in sprint planning, stand-ups, reviews, and retrospectives.

**Quality improvement**

- Suggest process improvements.
- Encourage early reviews that help prevent defects.
- Support CI/CD pipelines with automated checks.

### 4.6 Common QA tools

| Purpose | Examples |
|---|---|
| Bug tracking | Jira, Bugzilla |
| Test management | TestRail, Zephyr |
| Web automation | Selenium, Cypress, Playwright |
| API testing | Postman, REST Assured |
| Performance testing | JMeter, k6 |
| Mobile testing | Appium |
| CI/CD | Jenkins, GitHub Actions |

### 4.7 Key skills

- Attention to detail
- Analytical and logical thinking
- Clear written communication
- Basic programming in Java, Python, or JavaScript
- SQL basics for checking data
- Understanding of the Software Development Life Cycle (SDLC)
- Familiarity with Agile and Scrum

### 4.8 QA vs. testing vs. quality control

- **Quality Assurance (QA):** Process-focused; aims to prevent defects and improve how software is developed.
- **Quality Control (QC):** Product-focused; checks whether the product meets quality requirements.
- **Testing:** A set of activities used to evaluate software and discover defects.

In everyday software teams, these terms can overlap, and job titles do not always use them consistently.

### 4.9 Career path

A possible career path is:

**Junior QA Engineer → QA Engineer → Senior QA Engineer → QA Lead / QA Manager**

Alternative paths include:

- Software Development Engineer in Test (SDET)
- Test Automation Engineer
- Automation Architect
- DevOps or quality engineering roles

---

## 5. DevOps Engineer — Beginner Guide

**Version:** 1.0  
**Date:** October 2026  
**Audience:** Beginners who want to understand DevOps and start learning it step by step.

### 5.1 What Is DevOps?

**DevOps** combines **Development** and **Operations** practices to help teams build, test, release, deploy, and maintain software reliably.

- **Development:** Building and improving software applications.
- **Operations:** Running applications, managing infrastructure, monitoring services, and keeping systems reliable.
- **DevOps:** Improving collaboration and automating the path from code changes to a running application.

#### Example

Imagine a medicine information application with:

- **Frontend:** Next.js
- **Backend:** Go
- **Database:** PostgreSQL

Developers build the application, but it also needs to be configured, tested, deployed, monitored, and updated. DevOps practices help teams do these tasks consistently and automate repetitive steps.

### 5.2 What Does a DevOps Engineer Do?

Common responsibilities include:

1. Managing code workflows with Git and GitHub.
2. Packaging applications with Docker.
3. Automating builds, tests, and deployments with CI/CD.
4. Managing servers and cloud infrastructure.
5. Monitoring applications, logs, performance, and alerts.
6. Troubleshooting deployment and infrastructure problems.
7. Applying security practices to systems, credentials, and deployment pipelines.
8. Documenting infrastructure and release procedures.

The exact responsibilities vary by company. Some organizations have separate platform, cloud, security, and site reliability engineering teams.

### 5.3 Important DevOps Concepts and Tools

| Category | Examples | Purpose |
|---|---|---|
| Version control | Git, GitHub | Track code changes and collaborate |
| Operating systems | Linux | Manage servers and services |
| Networking | IP, DNS, HTTP/HTTPS, ports, firewalls | Understand how systems communicate |
| Containers | Docker | Package and run applications consistently |
| Multi-container development | Docker Compose | Run services together in a local environment |
| CI/CD | GitHub Actions | Automate checks, builds, and deployment steps |
| Cloud | AWS, Microsoft Azure, Google Cloud | Run applications and infrastructure |
| Infrastructure as Code | Terraform | Define infrastructure using configuration files |
| Container orchestration | Kubernetes | Manage containerized applications at scale |
| Scripting | Bash, Python | Automate repetitive tasks |
| Monitoring | Prometheus, Grafana, CloudWatch | Observe system health and performance |

**Important:** Do not try to learn every tool at once. Build a strong foundation first.

### 5.4 Git and GitHub

Git is a version-control tool. GitHub hosts Git repositories online and provides collaboration features such as issues, pull requests, reviews, and workflow automation.

#### Useful commands

```bash
git --version
git status
git add .
git commit -m "Describe the change"
git switch -c feature/example
git push -u origin feature/example
git pull
git log --oneline
git diff
```

These commands assume Git is configured and the repository has the appropriate remote. Set up your Git identity and remote repository if needed.

#### Typical team workflow

1. Create or receive an issue describing the task.
2. Create a branch for the task.
3. Make a small, focused change.
4. Commit and push the change.
5. Open a pull request.
6. Review and test the change.
7. Merge according to the team's process.

**Security tip:** Never commit passwords, API keys, tokens, private keys, or real `.env` files.

### 5.5 Linux Basics

Linux is widely used on servers and in cloud environments. DevOps engineers often use a terminal to inspect files, processes, services, and logs.

| Command | Purpose |
|---|---|
| `pwd` | Show the current directory |
| `ls -la` | List files, including hidden files |
| `cd folder` | Change directory |
| `mkdir demo` | Create a directory |
| `cat file.txt` | Display a file's contents |
| `grep "error" app.log` | Search a log for text |
| `ps aux` | List running processes |
| `df -h` | Show disk space usage |
| `free -h` | Show memory usage |
| `ss -tuln` | Show listening network sockets |

Practise in a test environment. Be cautious with commands that delete files, change permissions recursively, or modify system configuration. Use `sudo` only when necessary.

### 5.6 Networking Basics

Learn these concepts before moving deeply into cloud infrastructure:

- **IP address:** Identifies a device or network interface.
- **DNS:** Resolves domain names to IP addresses.
- **HTTP/HTTPS:** Protocols used by web applications; HTTPS protects data in transit using TLS.
- **Ports:** Identify network services on a host.
- **Firewall:** Controls allowed network traffic.
- **Router:** Forwards traffic between networks.
- **VPN:** Creates a protected connection across a network.
- **Client-server architecture:** A client requests a service from a server.

#### Safe commands to inspect your own device

Windows:

```powershell
ipconfig
nslookup example.com
netstat -ano
```

Linux:

```bash
ip addr
ip route
ss -tuln
ping -c 4 example.com
```

### 5.7 Docker and Docker Compose

Docker helps package applications and their dependencies into images and run them as containers.

- **Image:** A packaged template used to create containers.
- **Container:** A running instance of an image.
- **Dockerfile:** Instructions for building an image.
- **Volume:** Storage that can persist beyond a container's lifecycle.
- **Network:** Allows containers to communicate.
- **Docker Compose:** Defines and runs multiple services together.

#### Common commands

```bash
docker --version
docker pull nginx
docker run --name demo-web -p 8080:80 -d nginx
docker ps
docker logs demo-web
docker stop demo-web
docker rm demo-web
docker images
```

With the container running, open [http://localhost:8080](http://localhost:8080) in your browser.

#### Minimal Docker Compose example

Create a file named `compose.yaml`:

```yaml
services:
  web:
    image: nginx:alpine
    ports:
      - "8080:80"
```

Run it:

```bash
docker compose up -d
docker compose ps
docker compose logs
docker compose down
```

This example runs a simple web server. It is not a complete application stack.

### 5.8 CI/CD with GitHub Actions

**CI — Continuous Integration:** Code changes are integrated and checked automatically, often by running linting and tests.

**CD — Continuous Delivery or Continuous Deployment:** Validated changes are prepared for release or automatically deployed, depending on the pipeline.

A typical pipeline looks like this:

```text
Developer changes code
        |
        v
Push to GitHub / Open Pull Request
        |
        v
Automated checks and tests
        |
        v
Build application
        |
        v
Approval or release rules
        |
        v
Deploy application
        |
        v
Health checks and monitoring
```

#### Minimal workflow example

Create `.github/workflows/hello.yml`:

```yaml
name: Hello CI

on:
  push:
  pull_request:

jobs:
  check:
    runs-on: ubuntu-latest
    steps:
      - name: Check out code
        uses: actions/checkout@v4
      - name: Show a message
        run: echo "Workflow is running"
```

This workflow demonstrates that GitHub Actions runs; it does not test or deploy an application. For a real project, add the correct language setup, dependency installation, linting, tests, and build commands.

### 5.9 Cloud Computing

Cloud providers offer compute, storage, networking, databases, and monitoring services.

Common topics to learn:

- Virtual machines and compute services
- Networking and firewall rules
- Storage
- Identity and Access Management (IAM)
- Managed databases
- Environment variables and secrets
- Logs, monitoring, backups, and recovery
- Billing and cost controls

#### Example deployment choices

| Component | Possible hosting approach |
|---|---|
| Next.js frontend | A frontend platform or a server/container appropriate for its rendering mode |
| Go API | A container platform, virtual machine, or managed application service |
| PostgreSQL | A managed database or a securely managed server |
| Static files | Static hosting or object storage |

Before deploying, protect database access, use HTTPS, store secrets securely, configure backups, and check current pricing. Cloud services can create charges even when a project is only for learning.

### 5.10 Monitoring and Troubleshooting

Deployment is not the end of the process. Applications must be monitored and maintained.

Questions to investigate include:

- Is the application running?
- Is the server out of disk space or memory?
- Is CPU usage unusually high?
- Are API errors increasing?
- Can the backend connect to the database?
- What do the logs show?

Start with application logs, Docker logs, basic health checks, and cloud monitoring. Later, explore tools such as Prometheus and Grafana.

A useful troubleshooting approach is:

1. Identify the exact error and when it started.
2. Check logs and recent changes.
3. Test each component separately.
4. Verify network access and configuration.
5. Make one controlled change at a time.
6. Confirm the fix and document what happened.

### 5.11 Security Basics for DevOps

Security must be considered throughout development and deployment.

- Never store secrets in source control.
- Use least-privilege access.
- Keep operating systems, dependencies, and container images updated.
- Avoid exposing internal services or database ports publicly.
- Use HTTPS for public applications.
- Configure backups and test recovery.
- Protect CI/CD credentials and restrict workflow permissions.
- Review logs and rotate credentials if they may have leaked.

### 5.12 Practical Portfolio Project

#### Project: Medicine Information Application

Suggested technology stack:

| Component | Technology |
|---|---|
| Frontend | Next.js |
| Backend | Go |
| Database | PostgreSQL |
| Version control | Git and GitHub |
| Local containers | Docker and Docker Compose |
| CI/CD | GitHub Actions |
| Hosting | A suitable cloud or application hosting platform |

#### Project steps

1. Create a GitHub repository and document the setup in `README.md`.
2. Build a small Next.js frontend and Go API.
3. Create a PostgreSQL schema or migrations.
4. Run the components locally and verify their connections.
5. Add Dockerfiles and a Compose configuration.
6. Add GitHub Actions to run automated checks and tests.
7. Deploy the application using suitable hosting services.
8. Configure environment variables and protect secrets.
9. Check logs, HTTPS, database access, backups, and costs.
10. Document how to deploy, troubleshoot, and recover the application.

Suggested repository layout:

```text
my-project/
  web/                    # Next.js frontend
  server/                 # Go API
  database/               # Schema or migrations
  .github/workflows/      # CI workflows
  compose.yaml
  README.md
  .gitignore
```

Use `.env.example` for safe placeholder variable names. Keep real secrets in ignored environment files or an appropriate secret manager.

### 5.13 Suggested Four-Week Learning Plan

| Week | Focus | Practical outcome |
|---|---|---|
| 1 | Git, GitHub, Linux, networking basics | Create a repository, branch, pull request, and practise terminal commands |
| 2 | Docker and Docker Compose | Run a web server and a small local service stack |
| 3 | CI/CD with GitHub Actions | Run automated checks on each pull request |
| 4 | Cloud and monitoring basics | Deploy a small app, inspect logs, and document recovery steps |

This is a starting plan, not a guarantee of job readiness. Repeat the exercises and build projects until you can explain and troubleshoot them confidently.

### 5.14 Advanced Topics to Learn Later

After the fundamentals are comfortable, explore:

- **Terraform:** Infrastructure as Code.
- **Kubernetes:** Container orchestration.
- **Advanced CI/CD:** Deployment strategies, approvals, and rollback.
- **Observability:** Metrics, logs, traces, and alerting.
- **Cloud security:** IAM, network controls, secrets, and audit logs.
- **Site Reliability Engineering (SRE):** Reliability goals, service-level indicators, and incident learning.

Do not start with Kubernetes just because it is popular. Learn Linux, networking, Docker, and CI/CD first.

### 5.15 Quick Command Cheat Sheet

```bash
# Git
git status
git add .
git commit -m "Describe the change"
git switch -c feature/example
git push -u origin feature/example

# Linux
pwd
ls -la
cd folder
grep "error" app.log
ps aux
df -h

# Docker
docker ps
docker logs <container>
docker stop <container>
docker compose up -d
docker compose down
```

### 5.16 Official Documentation

- Git: [https://git-scm.com/doc](https://git-scm.com/doc)
- GitHub Docs: [https://docs.github.com/](https://docs.github.com/)
- Docker Docs: [https://docs.docker.com/](https://docs.docker.com/)
- GitHub Actions: [https://docs.github.com/actions](https://docs.github.com/actions)
- AWS Getting Started: [https://aws.amazon.com/getting-started/](https://aws.amazon.com/getting-started/)
- Terraform Documentation: [https://developer.hashicorp.com/terraform/docs](https://developer.hashicorp.com/terraform/docs)
- Kubernetes Documentation: [https://kubernetes.io/docs/](https://kubernetes.io/docs/)

### Final Advice

Learn one tool at a time, practise it, and write down what you did. A small project that you can explain and troubleshoot is more valuable than a long list of tools you have only installed.

---

## 6. Key Takeaways

- UI/UX design helps make digital products clear, accessible, and easy to use.
- Software architecture describes a system's structure and how its parts interact.
- AI engineering combines AI capabilities with application development, deployment, monitoring, and safety.
- QA engineering helps prevent defects and provides evidence about software quality.
- DevOps automates and standardizes how software is built, deployed, and monitored.
- Communication, teamwork, clear documentation, and continuous learning are valuable across all five areas.

## 7. Reflection

**What I learned:**  
Add the most important concepts learned during the session.

**What I found difficult:**  
Add concepts or tools that need more practice.

**What I will do next:**  
List a topic to research, a tool to try, or a small practical exercise to complete.
