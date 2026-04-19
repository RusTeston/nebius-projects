# AI & Infrastructure Glossary — Plain-English Edition

> A comprehensive, plain-English glossary of AI, cloud, container, and machine learning infrastructure terms. Every term includes an official definition, an everyday analogy, and its business purpose. Terms marked **[NEW]** were added in this expanded edition.

**Use the HTML version** (`Claude_Glossary_Term_Project.html`) for live search and A–Z filtering with highlighted results.

---

## Sources

- https://docs.nebius.com/
- https://docs.nebius.com/kubernetes
- https://docs.nebius.com/compute/clusters/gpu
- https://docs.nebius.com/serverless/overview
- https://docs.nebius.com/slurm-soperator
- https://docs.nebius.com/observability/logging
- https://nebius.com/
- https://nebius.com/services/managed-kubernetes
- https://nebius.com/solutions/inference
- https://nebius.com/blog

---

## A–Z Index

[A](#a) | [B](#b) | [C](#c) | [D](#d) | [E](#e) | [F](#f) | [G](#g) | [H](#h) | [I](#i) | [J](#j) | [K](#k) | [L](#l) | [M](#m) | [N](#n) | [O](#o) | [P](#p) | [Q](#q) | [R](#r) | [S](#s) | [T](#t) | [U](#u) | [V](#v) | [W](#w) | [X](#x) | [Y](#y) | [Z](#z)

---

## A

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **A/B Testing** | A method of comparing two versions of a model or system in production to see which performs better on real traffic. | Like trying two sales scripts with different customers to see which one closes more deals. | Reduces guesswork and improves model quality, conversion, or user experience before a full rollout. |
| **Accelerator** *(New)* | Specialized hardware—such as a GPU or TPU—designed to speed up specific compute tasks like matrix math used in AI training. | Like swapping a regular kitchen knife for a professional mandoline slicer: the same task, done 100× faster. | Cuts training and inference time dramatically, reducing cost and time-to-market for AI products. |
| **Agent (AI)** *(New)* | An AI system that takes sequences of actions autonomously—browsing the web, calling tools, or writing code—to complete a goal. | Like a personal assistant who doesn't just answer questions but actually books flights and sends emails on your behalf. | Enables automation of complex multi-step business tasks that previously required human operators. |
| **Apache Spark** | A distributed data processing engine for large-scale analytics and data engineering workloads. | Like a warehouse crew splitting a huge sorting job across many workers at once. | Speeds up large data preparation and analytics jobs that feed AI and reporting. |
| **API** | Application Programming Interface: a defined way for software systems to send requests to and receive responses from another service. | Like a restaurant menu and waiter: you order in a standard way and the kitchen delivers it. | Lets teams connect apps, automate workflows, and use AI services without manual steps. |
| **Attention Mechanism** *(New)* | A component inside transformer models that lets the model focus on relevant parts of the input when generating each output token. | Like a reader who highlights the most important sentences before answering a quiz question. | Is the core innovation that makes large language models powerful enough for complex reasoning and generation. |
| **Autoscaling** | The automatic increase or decrease of computing resources based on workload demand. | Like opening more checkout lanes when the store gets busy, then closing them when traffic drops. | Helps control cost while maintaining performance during traffic spikes. |

---

## B

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Batch Inference** | Running model predictions on a large collection of data items as a job rather than responding one request at a time. | Like grading a whole stack of tests overnight instead of answering one student at a time. | Useful for offline scoring, reporting, content processing, and other non-real-time tasks. |
| **Batch Job** | A non-interactive task that runs to completion and usually processes data or compute work in the background. | Like dropping off laundry and picking it up when the cleaning is done. | Ideal for scheduled processing, training, evaluation, and large one-time workloads. |
| **Batch Script** | A shell script that defines how a batch job should run, including commands and requested resources. | Like a written work order telling a crew exactly what to do and what tools they need. | Makes compute jobs repeatable, consistent, and easier to automate. |
| **Blackwell GPU** | NVIDIA's Blackwell generation of accelerated computing hardware referenced for self-service AI clusters. | Like a newer, faster engine model in the same family of sports cars. | Offers more performance for advanced model training and inference workloads. |
| **Blueprint** | In NVIDIA Blueprint, a packaged workflow combining multiple AI steps into a ready starting point. | Like a meal kit that includes the ingredients and recipe for a complex dinner. | Speeds up deployment by giving teams a preassembled workflow instead of starting from scratch. |
| **Boot Disk Image** | A prebuilt disk template used to start a virtual machine with a chosen operating system and software stack. | Like buying a laptop with the operating system and core apps already installed. | Cuts setup time and helps standardize environments across teams. |

---

## C

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Checkpoint** *(New)* | A saved snapshot of a model's weights at a point during training so work can be resumed or the model version reused later. | Like hitting "Save" in a video game so you don't lose hours of progress if something goes wrong. | Protects expensive training runs from loss and enables teams to roll back to earlier, better-performing model versions. |
| **CLI** | Command-Line Interface: a text-based way to create, inspect, and manage cloud resources. | Like giving precise instructions at a drive-through speaker instead of tapping buttons on a kiosk. | Useful for automation, scripting, repeatability, and fast power-user workflows. |
| **Cluster** | A group of connected compute resources that work together as one system. | Like a team of workers assigned to one big project instead of one person doing it all. | Enables scale, resilience, and parallel processing for demanding AI jobs. |
| **Context Window** *(New)* | The maximum number of tokens (words/pieces) a language model can read and consider at one time when generating a response. | Like the width of a desk — it determines how many pages you can spread out and reference at once while working. | Larger context windows let AI handle longer documents, conversations, and code files without losing information. |
| **Container** | A lightweight package that includes an application and all the software it needs to run consistently across environments. | Like packing a food order in a sealed box with everything needed inside. | Improves portability, consistency, and deployment speed. |
| **Containerized Application** | An application packaged and run inside a container. | Like shipping a mobile coffee stand that arrives with the espresso machine and supplies already inside. | Makes software easier to move between laptops, servers, and cloud platforms. |
| **Controller Node** | In a Slurm/Soperator setup, the node that manages scheduling and orchestration of jobs. | Like an air traffic controller directing planes to the right runways and gates. | Coordinates work so jobs start in the right place at the right time. |
| **CPU** *(New)* | Central Processing Unit: the general-purpose processor in a computer that handles most instructions and logic sequentially. | Like a single brilliant chef who can cook anything but can only work on one dish at a time. | Handles coordination, business logic, and lighter workloads; GPU handles the heavy parallel math for AI. |
| **CUDA** | NVIDIA's parallel computing platform and programming model for running workloads on GPUs. | Like giving chefs a special kitchen layout so they can cook many dishes at once very efficiently. | Lets developers accelerate training, inference, and scientific computing on NVIDIA GPUs. |

---

## D

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Data Lake** *(New)* | A centralized repository that stores raw, unstructured, and structured data at any scale until it is needed for analysis or training. | Like a massive warehouse where you toss everything you own — you can find and use anything later, but it takes some digging. | Enables organizations to capture all data now and decide how to use it for AI or analytics later. |
| **Data Pipeline** *(New)* | An automated series of steps that moves, transforms, and loads data from its source to its destination for use in AI or analytics. | Like an assembly line that takes raw materials at one end and delivers finished, packaged products at the other. | Ensures clean, timely data reaches training and inference systems without manual intervention. |
| **Data Preprocessing** | Cleaning, transforming, and organizing raw data before using it for training or inference. | Like washing, peeling, and chopping ingredients before cooking. | Improves model accuracy and reliability by feeding cleaner input into the pipeline. |
| **Deployment** *(New)* | The process of releasing a trained model or application into a production environment where real users or systems can access it. | Like opening a restaurant after months of recipe testing — the kitchen is finally serving real customers. | Turns model development into business value by making AI accessible to end users or downstream systems. |
| **Device Plugin** | A Kubernetes component that exposes specialized hardware, such as GPUs, to workloads running in the cluster. | Like a valet system that tells guests which specialty vehicles are actually available. | Allows containers to use scarce hardware resources in a controlled way. |
| **Distributed Training** | Training a model across multiple GPUs or machines working together. | Like several construction crews building different parts of the same stadium at the same time. | Shortens training time for large models and datasets. |
| **Docker** | A widely used container platform for building, packaging, and running containerized applications. | Like a standard brand of shipping container that works on many trucks, ships, and ports. | Makes application packaging and deployment more predictable and portable. |

---

## E

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Embedding** *(New)* | A numerical vector that represents text, images, or other data in a way that captures meaning, so similar things end up near each other mathematically. | Like converting book summaries into GPS coordinates — books with similar themes end up geographically close together on a map. | Powers semantic search, recommendation engines, and retrieval-augmented AI by enabling similarity comparisons. |
| **Endpoint** | In Serverless AI, an interactive service that listens for requests and returns model responses until stopped. | Like a staffed service desk that stays open to answer incoming questions. | Supports real-time AI experiences such as chat, search, and live predictions. |
| **Epoch** *(New)* | One complete pass through the entire training dataset by the model during the learning process. | Like reading a textbook from cover to cover once — multiple epochs means reading it multiple times to absorb more. | More epochs improve model accuracy up to a point; too many cause overfitting, so monitoring epochs is essential. |

---

## F

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Fault Tolerance** | The ability of a system to keep operating even when some parts fail. | Like a restaurant staying open because another cook can step in when one calls out sick. | Improves uptime and user trust by reducing outages. |
| **Fine-Tuning** | Adapting a pre-trained model to a narrower task or dataset by continuing training on new examples. | Like taking a general athlete and coaching them for one specific sport. | Improves relevance and quality for a company's specific use case. |
| **Foundation Model** *(New)* | A large model trained on broad data at scale that can be adapted to many downstream tasks through fine-tuning or prompting. | Like a general-purpose Swiss Army knife — it does many things reasonably well out of the box. | Reduces the cost of building AI capabilities by letting businesses start from a powerful, reusable base instead of training from scratch. |
| **Framework** | A reusable software foundation that provides structure and common components for building applications. | Like the frame of a house that gives builders a standard structure to work with. | Speeds development and reduces custom reinvention. |

---

## G

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **GenAI** | Generative AI: systems that create new content such as text, images, code, or audio. | Like a creative assistant that drafts new material instead of only retrieving old files. | Enables products like copilots, chatbots, content tools, and design assistants. |
| **GlusterFS** | A distributed file system referenced by Nebius solution examples for shared storage across cluster nodes. | Like a shared company filing room that many teams can access from different offices. | Helps multiple machines read and write shared data needed by training jobs. |
| **GPU** | Graphics Processing Unit: a processor built to handle many calculations in parallel, making it well suited for AI workloads. | Like having hundreds of prep cooks working at once instead of one chef doing everything. | Accelerates training, inference, and data processing workloads that would be too slow on general-purpose chips. |
| **GPU Cluster** | A cluster of machines or nodes equipped with GPUs and connected to work together on heavy workloads. | Like a fleet of tow trucks working the same major recovery job. | Provides the scale needed for large model training and high-throughput inference. |
| **GPU Driver** | System software that lets the operating system and applications communicate correctly with the GPU. | Like the translator between the driver and a very specialized race car. | Required to make GPU hardware usable and stable for AI workloads. |
| **Grafana** | A visualization tool used for dashboards that display metrics and system health. | Like a control-room wall of gauges and screens showing how the factory is running. | Helps teams monitor performance, spot anomalies, and troubleshoot faster. |
| **Guardrails** *(New)* | Rules, filters, or checks placed around an AI model to prevent it from generating harmful, off-topic, or policy-violating outputs. | Like the bumpers in bumper bowling — they guide the ball and stop it from going somewhere it shouldn't. | Protects brand, users, and legal compliance by keeping AI outputs within acceptable boundaries. |

---

## H

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Hallucination** *(New)* | When an AI model confidently generates text that sounds plausible but is factually wrong or entirely made up. | Like a tour guide confidently describing landmarks that don't exist — spoken fluently and convincingly. | One of the biggest risks in enterprise AI deployment; mitigated by grounding models in real data via RAG or fact-checking layers. |
| **Helm** *(New)* | A package manager for Kubernetes that bundles application definitions into reusable "charts" for easy deployment. | Like an App Store for Kubernetes — instead of building everything from scratch, you install pre-packaged software bundles. | Speeds up and standardizes how teams deploy complex applications and AI infrastructure components to Kubernetes. |
| **High Availability** | A design goal in which services are built to remain accessible with minimal downtime. | Like keeping a spare generator ready so the lights stay on when the power fails. | Protects revenue and operations by reducing service interruption. |
| **Horovod** *(New)* | An open-source distributed deep learning training framework that helps scale model training across many GPUs. | Like a relay race where each runner carries the baton for their leg — each GPU trains on part of the data and passes results to the others. | Reduces training time for large models by efficiently coordinating work across dozens or hundreds of GPUs. |
| **HPC** | High-Performance Computing: the use of powerful, often parallel systems to solve compute-intensive problems. | Like using an industrial bakery instead of a home oven when you need ten thousand loaves. | Supports large simulations, scientific workloads, and massive model training runs. |
| **Hyperparameter** *(New)* | A configuration value set before training begins — such as learning rate or batch size — that controls how the model learns. | Like the temperature and baking time settings you choose before putting bread in the oven — they shape the result without being part of the dough. | Tuning hyperparameters can dramatically improve model performance, and cloud platforms automate this search to save time. |

---

## I

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Infrastructure as Code (IaC)** *(New)* | The practice of defining and managing cloud infrastructure through machine-readable configuration files instead of manual setup. | Like a detailed recipe that automatically instructs a robot kitchen to cook the same meal perfectly every time. | Enables repeatable, auditable, version-controlled infrastructure deployments that reduce human error. |
| **Inference** | Using a trained model to generate predictions or outputs from new input data. | Like asking an experienced mechanic to identify a problem after years of training. | Turns trained models into usable products and business decisions. |
| **InfiniBand** | A high-throughput, low-latency networking technology used to connect systems for demanding compute workloads. | Like replacing neighborhood roads with a private high-speed express lane between factories. | Helps large GPU workloads exchange data faster, improving multi-node performance. |
| **Interactive Workload** | A workload that stays running and responds to incoming requests in real time. | Like a help desk agent who stays at the phone waiting for calls. | Supports user-facing services where fast response matters. |

---

## J

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Job Allocation** | The set of compute resources reserved by Slurm for a submitted job. | Like booking a meeting room, projector, and staff before an event starts. | Ensures the required resources are ready before the job runs. |
| **Job Queue** *(New)* | The ordered list of submitted compute jobs waiting for resources to become available before they can begin running. | Like a numbered ticket system at a deli — your job is assigned a number and gets called when it's its turn. | Enables fair, priority-based sharing of expensive GPU resources across multiple teams or projects. |
| **Job Scheduler** | Software that decides when and where compute jobs should run based on rules and available resources. | Like a dispatcher assigning delivery routes to available drivers. | Improves utilization, fairness, and throughput in shared compute environments. |
| **Jupyter Notebook** *(New)* | An interactive web-based environment where data scientists and developers can write and run code, visualize results, and document their work in one place. | Like a live science lab notebook where you can run experiments and record results on the same page. | Accelerates AI experimentation and model prototyping, and makes analytical work shareable across teams. |

---

## K

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **kubectl** | The native command-line tool used to work with Kubernetes clusters. | Like the remote control for a very large machine room. | Lets engineers inspect, update, and troubleshoot Kubernetes resources efficiently. |
| **Kubernetes** | An orchestration platform for deploying, scaling, and managing containerized applications. | Like an operations manager who decides where each shipping container goes and replaces broken trucks automatically. | Helps companies run AI and application workloads reliably at scale. |
| **KV Cache** *(New)* | A memory optimization in transformer inference that stores previously computed key-value pairs to avoid redundant recalculation on each new token. | Like a student keeping scratch work on the side of the page so they don't have to redo calculations every time they need the same number. | Dramatically speeds up inference for long conversations and documents, reducing cost per query. |

---

## L

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Latency** *(New)* | The time it takes for a system to respond to a request — from when input is sent to when output is received. | Like the wait between pressing the elevator button and the doors opening. | Low latency is critical for interactive AI applications; high latency degrades user experience and revenue. |
| **Llama** | A family of large language models referenced in Nebius fine-tuning examples. | Like a pre-trained writer you can coach for your specific brand voice. | Serves as a base model for custom AI assistants and other language applications. |
| **LLM** *(New)* | Large Language Model: an AI model trained on vast text data that can understand and generate human language for a wide variety of tasks. | Like a very well-read colleague who has processed millions of books, articles, and conversations and can discuss almost any topic. | Powers chatbots, copilots, summarization, coding assistants, and countless enterprise automation use cases. |
| **Login Node** | In a Slurm cluster, a node that users access to submit jobs and work with the environment. | Like the front desk and lobby where visitors arrive before going deeper into the building. | Provides a controlled entry point for users and workflows. |
| **LogQL** | A query language used for searching and analyzing logs in Loki-style systems. | Like a detective's search grammar for finding the right clues in a mountain of notes. | Helps teams quickly find errors, patterns, and operational signals in logs. |
| **Loki** | A log aggregation system often used alongside Grafana for storing and querying logs. | Like a searchable archive room for every machine and app message in the building. | Makes it easier to investigate incidents and understand system behavior. |

---

## M

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Managed Kubernetes** | Nebius's managed service for deploying and operating Kubernetes clusters with less manual overhead. | Like renting a serviced office where building management handles the plumbing and power. | Lets teams focus on applications instead of running every part of the cluster themselves. |
| **Microservice** *(New)* | A software design pattern where an application is broken into small, independent services that communicate via APIs. | Like a food hall where each stall specializes in one cuisine — each works independently but they all serve the same customers. | Allows AI components like inference, preprocessing, and logging to be scaled, updated, and maintained independently. |
| **MLflow** | An open-source platform for managing machine learning experiments and model lifecycle tasks. | Like a lab notebook mixed with a project tracker for model work. | Improves experiment tracking, reproducibility, and collaboration. |
| **ML/AI Workload** | A computing task related to machine learning or AI, such as training, inference, preprocessing, or evaluation. | Like the collection of jobs in a movie studio: filming, editing, sound, and release. | Helps teams categorize and optimize the kinds of compute work they run. |
| **MLOps** *(New)* | Machine Learning Operations: the practices and tools for deploying, monitoring, and maintaining ML models in production reliably. | Like having a dedicated pit crew for race cars — they keep the car running, swap tires, and ensure it stays competitive lap after lap. | Bridges the gap between model development and production, reducing the time and risk of getting AI into business systems. |
| **Model Evaluation** | Testing a model to measure how well it performs on defined tasks or datasets. | Like giving a student a final exam after months of study. | Prevents weak models from reaching customers and supports governance. |
| **Model Registry** *(New)* | A centralized store where trained model versions are tracked, versioned, and managed across their lifecycle. | Like a library catalog — each book (model) is catalogued with its edition, where it came from, and who checked it out. | Ensures teams can trace model lineage, roll back to stable versions, and comply with AI governance requirements. |
| **Monitoring** | Collecting and viewing metrics, events, and health data about infrastructure and applications. | Like checking vital signs on a hospital monitor. | Helps teams detect issues early and keep services reliable. |
| **Multi-Host Training** | Training that spans multiple machines rather than a single server. | Like splitting a giant warehouse order across several fulfillment centers. | Needed when one machine does not have enough compute or memory for the job. |
| **Multi-Node Workload** | A job that runs across multiple nodes in a cluster. | Like a film production spread across several stages but following one production plan. | Allows larger or faster processing than a single node can provide. |

---

## N

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Namespace** *(New)* | A virtual partition inside a Kubernetes cluster that isolates resources, allowing multiple teams or environments to share the same cluster safely. | Like separate floors in a shared office building — different companies share the structure but have their own locked space. | Enables safe multi-tenant cluster usage and helps enforce resource quotas and access controls per team. |
| **Nebius AI Cloud** *(New)* | A cloud platform purpose-built for AI workloads, offering GPU compute, managed Kubernetes, Slurm-based HPC, and AI-focused infrastructure services. | Like a specialty workshop fully equipped for auto restoration — built specifically for that craft, not a general rental space. | Provides AI and ML teams with optimized, cost-effective infrastructure without managing raw hardware. |
| **NIM (NVIDIA)** *(New)* | NVIDIA Inference Microservices: containerized, optimized model servers that make it easy to deploy AI models at production scale. | Like a pre-assembled, road-tested food truck — the engine, kitchen, and menu are ready; you just choose where to park it. | Speeds time-to-production for AI inference by providing optimized serving containers from NVIDIA. |
| **Node** | A single machine or compute instance that participates in a cluster. | Like one employee on a larger team. | Serves as a building block for scalable systems. |
| **Node Group** | A set of similar nodes managed together inside a Kubernetes cluster. | Like a department made up of employees with the same role and equipment. | Makes it easier to scale and manage groups of machines consistently. |
| **NVLink** | NVIDIA's high-speed interconnect for moving data efficiently between GPUs. | Like a private hallway between offices instead of sending everything through the public street. | Improves performance when multiple GPUs need to share data rapidly. |

---

## O

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Object Storage** *(New)* | A type of cloud storage that keeps data as discrete objects (files + metadata) in a flat namespace, ideal for large unstructured data like datasets and model artifacts. | Like a massive self-storage facility where each unit is labeled with a unique number — you can retrieve any item instantly if you know its number. | Cost-effective way to store huge training datasets, model checkpoints, and output files at scale. |
| **Observability** | The practice of understanding system health by using metrics, logs, traces, and related signals. | Like not just checking that a car is on, but also having the dashboard, service log, and engine diagnostics. | Speeds troubleshooting and improves operational reliability. |
| **Operator** | In Kubernetes, software that automates the deployment and lifecycle management of complex applications. | Like a specialist caretaker who knows how to install, tune, heal, and upgrade a specific machine. | Reduces manual administration and enforces best practices. |
| **Orchestration** | Coordinating many compute resources and workloads so they run in the right place and order. | Like a conductor keeping an orchestra in sync. | Essential for scaling AI systems efficiently and reliably. |
| **Overfitting** *(New)* | When a model learns training data too precisely — including its noise — and fails to generalize to new, unseen data. | Like a student who memorizes every practice test answer verbatim but can't solve a slightly rephrased question on the real exam. | A common AI quality failure; avoided with techniques like regularization, dropout, and proper data splitting. |

---

## P

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Parallel Computing** | Using many processors or cores at the same time to solve parts of a problem together. | Like having many people assemble different sections of the same puzzle simultaneously. | Cuts runtime for large workloads and makes advanced AI feasible. |
| **Parameter** *(New)* | A single numerical value inside a model that is learned during training; models are often described by their parameter count (e.g., 7 billion). | Like individual adjustable screws inside a complex machine — each one affects how the machine behaves, and training tunes them all. | Parameter count signals model capability and resource requirements; more parameters generally means more power but higher cost. |
| **Pod** | The basic deployable unit in Kubernetes that runs one or more tightly coupled containers. | Like a small work booth that can hold one specialist or a tiny team that must travel together. | Provides a practical unit for scheduling, scaling, and managing applications. |
| **PostgreSQL** | An open-source relational database system. | Like a very organized digital filing cabinet with strong rules for storing and finding records. | Supports applications that need reliable structured data storage. |
| **Pretraining** *(New)* | The initial phase of training a foundation model on a massive, broad dataset to give it general knowledge and language understanding. | Like putting a new hire through a comprehensive multi-year university education before they start their specialized role. | Creates the general-purpose capability that makes models like LLMs useful across many tasks without task-specific data. |
| **Project** | In Nebius, a resource boundary used to organize and control related cloud resources. | Like a labeled folder that keeps one department's budget, assets, and paperwork together. | Helps with organization, access control, and billing separation. |
| **Prometheus** | A monitoring system that collects and stores metrics from infrastructure and applications. | Like an automated clipboard that records performance readings at regular intervals. | Gives teams the data needed for dashboards, alerting, and capacity planning. |
| **Prompt** *(New)* | The input text or instruction given to an AI model that tells it what task to perform or question to answer. | Like giving a briefing to a contractor — the clearer and more detailed your instructions, the better the outcome. | Prompt quality directly affects AI output quality; well-crafted prompts are a core enterprise skill for AI adoption. |
| **Provisioning** | Creating and configuring infrastructure resources so they are ready to use. | Like setting up desks, laptops, and badges before a new team arrives. | Speeds onboarding of systems and supports automation. |
| **PyTorch** *(New)* | An open-source deep learning framework widely used for model research and production training, especially in AI labs. | Like a professional woodworking kit — flexible, precise, and favored by craftspeople who need full control. | The dominant framework for training state-of-the-art AI models; knowing its infrastructure requirements is key for cloud planning. |

---

## Q

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Quantization** *(New)* | A technique that reduces the numerical precision of a model's weights to make it smaller and faster, with minimal accuracy loss. | Like compressing a high-resolution photo to a smaller file size — it looks almost the same but takes up far less space. | Allows large models to run on less expensive hardware or edge devices, dramatically reducing inference cost. |
| **Queue Depth** | The number of requests or tasks waiting to be processed. | Like the number of people lined up at a coffee shop. | A useful signal for scaling systems and detecting bottlenecks. |

---

## R

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **RAG** *(New)* | Retrieval-Augmented Generation: a pattern where an AI model retrieves relevant external documents at query time and uses them to ground its response. | Like an open-book exam — instead of relying only on memory, the model is allowed to look things up before answering. | Reduces hallucination and keeps AI responses accurate and up-to-date without expensive retraining. |
| **Real-Time Inference** | Producing model outputs immediately in response to live requests. | Like a translator speaking right as someone talks. | Important for chatbots, fraud checks, recommendations, and interactive apps. |
| **Region** | A geographic cloud location where resources run. | Like choosing which city to open a branch office in. | Affects latency, compliance, disaster planning, and service availability. |
| **RLHF** *(New)* | Reinforcement Learning from Human Feedback: a technique for training AI models to produce outputs that align with human preferences using rated example responses. | Like coaching an employee by having managers rate their work and rewarding them when they get it right. | The key method used to make LLMs helpful, harmless, and honest — critical for safe enterprise AI deployment. |
| **Rollout Strategy** *(New)* | The plan for releasing a new model or service version to users — such as gradual canary releases or full blue/green switches. | Like a restaurant testing a new menu item with just 10% of tables before rolling it out everywhere. | Minimizes risk by catching problems with a small user group before they affect everyone. |

---

## S

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Sbatch** | A Slurm command used to submit a batch script for execution. | Like handing a completed work order to the dispatcher. | Standardizes how jobs are submitted to the scheduler. |
| **Scheduling** | The process of assigning jobs to available resources over time. | Like deciding which meeting gets which room and when. | Keeps shared infrastructure efficient and fair. |
| **Serverless AI** | Nebius's service model for running AI endpoints or jobs without managing the underlying servers directly. | Like catering a meal without renting and staffing the kitchen yourself. | Speeds delivery and reduces operational overhead for AI teams. |
| **Service Account** | A non-human identity used by applications or automation to access cloud resources. | Like a company badge issued to a robot worker instead of a person. | Improves security and automation by separating app permissions from user accounts. |
| **Shared Filesystem** | A storage system that multiple machines can access as a common file space. | Like a shared drive everyone on a team can open. | Important for training data, checkpoints, and collaboration across nodes. |
| **Shared Responsibility Model** | A cloud security principle where the provider secures some layers and the customer secures others. | Like a landlord handling the building structure while the tenant locks their own office. | Clarifies who is responsible for security, compliance, and operations. |
| **SkyPilot** *(New)* | An open-source framework referenced by Nebius that automates launching AI and ML jobs across cloud providers and Kubernetes clusters. | Like a universal flight booking agent that finds the cheapest and fastest available flight regardless of airline. | Helps organizations minimize compute cost and maximize GPU availability across cloud platforms. |
| **Slurm** | An open-source workload manager and job scheduler widely used for high-performance computing and AI training. | Like a factory foreman assigning heavy jobs to the right crews and machines. | Helps organizations run large batch and training workloads efficiently. |
| **Soperator** | Nebius's open-source Kubernetes operator that runs Slurm nodes as Kubernetes Pods, combining Slurm and Kubernetes in one infrastructure. | Like mounting a factory foreman inside a modern operations control center so both work together. | Brings familiar Slurm job workflows to Kubernetes-based infrastructure. |
| **Srun** | A Slurm command used to launch tasks or job steps inside an allocated job. | Like telling individual crew members to start their part of the work after the site is reserved. | Supports multi-step and multi-node execution inside scheduled jobs. |
| **System Prompt** *(New)* | A set of instructions given to an AI model at the start of a session that defines its role, behavior, and constraints throughout the conversation. | Like a job description and employee handbook given to a new hire on day one — it shapes how they respond to everything. | Lets businesses customize AI behavior for specific use cases like customer service, coding help, or legal review. |

---

## T

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Temperature** *(New)* | A parameter that controls how random or creative an AI model's outputs are — low temperature means predictable, high temperature means more varied. | Like a dial on a blender — low speed gives controlled, consistent results; high speed mixes things up wildly. | Lets businesses tune AI behavior: low temperature for factual tasks, higher for brainstorming and creative work. |
| **Tensor** *(New)* | A multi-dimensional array used as the fundamental data structure in deep learning to represent everything from images to text embeddings. | Like a spreadsheet that can have many dimensions — not just rows and columns, but stacks of pages deep. | All data flowing through a neural network is a tensor; understanding tensors is foundational to AI infrastructure planning. |
| **Terraform** | An infrastructure-as-code tool used to define and provision cloud resources from configuration files. | Like an architect's blueprint that can automatically assemble the building crew's work orders. | Improves repeatability, version control, and automation for infrastructure. |
| **Throughput** *(New)* | The number of requests, tasks, or tokens a system can process per unit of time. | Like how many cars per hour a toll booth can process — it defines the capacity of the system. | Higher throughput means more AI queries served at lower cost; critical for high-volume production deployments. |
| **Token** *(New)* | The basic unit of text that an AI model reads and generates — typically a word or part of a word; models process and are priced by token count. | Like Scrabble tiles — text is broken into individual tiles before the model "plays" with them. | Token count drives inference cost and context window limits; understanding tokens helps budget AI API usage. |
| **Training** | The process of teaching a model by adjusting it using data so it can perform a task. | Like coaching a new employee through many examples until they get good at the job. | Creates the model capability that later powers AI products. |
| **Transformer** *(New)* | The dominant neural network architecture behind modern LLMs and vision models, based on the attention mechanism to relate all parts of an input to each other. | Like a team of editors who each read the entire document and highlight how every sentence relates to every other sentence. | Understanding the transformer architecture is foundational to AI infrastructure decisions, as it drives GPU memory and compute requirements. |
| **TPU** *(New)* | Tensor Processing Unit: Google's custom ASIC chip designed specifically to accelerate machine learning workloads, particularly matrix operations in neural networks. | Like a specialized espresso machine versus a general kitchen stove — purpose-built to do one thing exceptionally fast. | Offers an alternative to GPUs for large-scale AI training, with different cost/performance tradeoffs depending on workload. |

---

## U

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Utilization** *(New)* | The percentage of available compute resources (GPU, CPU, memory) actively being used at any moment. | Like how many seats in a restaurant are filled at dinner — low utilization means you're paying for empty tables. | High utilization means better return on expensive GPU infrastructure; monitoring utilization is key to cost optimization. |

---

## V

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Vector Database** *(New)* | A database designed to store and search vector embeddings efficiently, enabling fast similarity lookups across millions of items. | Like a music app that can find songs that "sound similar" to one you like — it's searching by feel, not by exact keyword. | Powers semantic search, RAG systems, and recommendation engines by enabling AI to find conceptually related content instantly. |
| **Virtual Machine (VM)** | A software-defined computer that runs its own operating system on shared physical hardware. | Like renting an apartment in a larger building: it feels like your own place even though the structure is shared. | Provides flexible isolated compute for apps, data jobs, and AI workloads. |
| **vLLM** *(New)* | An open-source high-throughput LLM serving engine that uses paged attention to dramatically increase GPU utilization during inference. | Like a highly efficient hotel concierge who handles many guests simultaneously instead of helping one at a time. | Reduces inference cost per query significantly and is widely used in production LLM deployments on platforms like Nebius. |

---

## W

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Worker Node** | A node that actually runs application workloads or Slurm jobs. | Like the production floor where the real manufacturing happens. | Provides the compute capacity that does the work. |
| **Workflow** | An ordered sequence of steps that together complete a task or process. | Like a recipe with stages from prep to cooking to plating. | Helps teams standardize complex AI and data operations. |
| **Workload Manager** | Software category that manages compute jobs and resource usage; Nebius discusses Slurm and Kubernetes in this role. | Like a dispatcher coordinating people, rooms, and equipment for many projects. | Improves utilization, scheduling, and operational control in shared environments. |

---

## X

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **XGBoost** *(New)* | An optimized gradient-boosting framework for training fast, accurate models on tabular (spreadsheet-style) data. | Like having a committee of specialists vote on each decision — their combined judgment is more accurate than any single expert. | Widely used for structured data predictions like fraud detection, churn, and pricing — often outperforms deep learning for tabular data. |

---

## Y

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **YAML** *(New)* | A human-readable configuration file format used extensively in Kubernetes, CI/CD pipelines, and infrastructure-as-code to define how systems should behave. | Like a plain-English instruction manual for machines — written in a way both humans and computers can understand. | The de facto format for configuring AI infrastructure in Kubernetes; every DevOps and MLOps team works with YAML daily. |

---

## Z

| Term | Official Definition | Easy Analogy | Business Purpose |
|---|---|---|---|
| **Zero-Downtime Deployment** *(New)* | A deployment strategy that updates a running service to a new version without any interruption in service for users. | Like repaving a highway by shifting traffic to one lane — the road keeps functioning while the work gets done. | Critical for production AI services where downtime means lost revenue and degraded user trust. |
| **Zero-Shot Learning** *(New)* | The ability of an AI model to perform a task it was never explicitly trained on, using only a description or prompt at inference time. | Like asking a multilingual professor to grade a paper in a language they've never formally studied — they use their general knowledge to figure it out. | Enables rapid prototyping of AI capabilities without needing labeled training data for every new task. |
