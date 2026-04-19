# Nebius AI & AI Infrastructure Glossary

Compiled from terminology and concepts surfaced across Nebius AI Cloud documentation, Nebius service pages, and Nebius technical blog content.

Use the HTML version for live search and A–Z filtering.

## Sources used
- https://docs.nebius.com/
- https://docs.nebius.com/kubernetes
- https://docs.nebius.com/kubernetes/gpu/set-up
- https://docs.nebius.com/compute/clusters/gpu
- https://docs.nebius.com/serverless/overview
- https://docs.nebius.com/slurm-soperator
- https://docs.nebius.com/slurm-soperator/overview/why-slurm-soperator
- https://docs.nebius.com/slurm-soperator/overview/architecture
- https://docs.nebius.com/slurm-soperator/jobs
- https://docs.nebius.com/slurm-soperator/clusters/connect
- https://docs.nebius.com/observability/logging
- https://docs.nebius.com/observability/logs/nebius-cli
- https://nebius.com/
- https://nebius.com/services/managed-kubernetes
- https://nebius.com/solutions/inference
- https://nebius.com/blog/posts/model-pre-training/slurm-vs-k8s
- https://nebius.com/blog/posts/how-to-use-kubernetes-for-ai-workloads
- https://nebius.com/blog/posts/ai-model-components-key-elements-of-a-genai-inference-setup-explained
- https://nebius.com/blog/posts/introducing-managed-soperator
- https://nebius.com/blog/posts/running-nvidia-nim-and-blueprint-on-nebius-ai-cloud
- https://nebius.com/blog/posts/skypilot-k8s-for-multi-node-fine-tuning

## A–Z Index

[A](#a) | [B](#b) | [C](#c) | [D](#d) | [E](#e) | [F](#f) | [G](#g) | [H](#h) | [I](#i) | [J](#j) | [K](#k) | [L](#l) | [M](#m) | [N](#n) | [O](#o) | [P](#p) | [Q](#q) | [R](#r) | [S](#s) | [T](#t) | [V](#v) | [W](#w)

## A

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **A/B testing** | A method of comparing two versions of a model or system in production to see which performs better on real traffic. | Like trying two sales scripts with different customers to see which one closes more deals. | Reduces guesswork and improves model quality, conversion, or user experience before a full rollout. |
| **Apache Spark** | A distributed data processing engine for large-scale analytics and data engineering workloads. | Like a warehouse crew splitting a huge sorting job across many workers at once. | Speeds up large data preparation and analytics jobs that feed AI and reporting. |
| **API** | Application Programming Interface: a defined way for software systems to send requests to and receive responses from another service. | Like a restaurant menu and waiter: you ask for something in a standard way, and the kitchen delivers it. | Lets teams connect apps, automate workflows, and use AI services without manual steps. |
| **Autoscaling** | The automatic increase or decrease of computing resources based on workload demand. | Like opening more checkout lanes when the store gets busy, then closing them when traffic drops. | Helps control cost while maintaining performance during traffic spikes. |

## B

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Batch inference** | Running model predictions on a large collection of data items as a job rather than responding one request at a time. | Like grading a whole stack of tests overnight instead of answering one student at a time. | Useful for offline scoring, reporting, content processing, and other non-real-time tasks. |
| **Batch job** | A non-interactive task that runs to completion and usually processes data or compute work in the background. | Like dropping off a pile of laundry and picking it up when the cleaning is done. | Ideal for scheduled processing, training, evaluation, and large one-time workloads. |
| **Batch script** | A shell script that defines how a batch job should run, including commands and requested resources. | Like a written work order telling a crew exactly what to do and what tools they need. | Makes compute jobs repeatable, consistent, and easier to automate. |
| **Blackwell GPU** | NVIDIA's Blackwell generation of accelerated computing hardware, referenced by Nebius for self-service AI clusters. | Like a newer, faster engine model in the same family of sports cars. | Offers more performance for advanced model training and inference workloads. |
| **Blueprint** | In NVIDIA Blueprint, a packaged workflow that combines multiple AI or scientific steps into a ready starting point. | Like a meal kit that includes the ingredients and recipe for a complex dinner. | Speeds up deployment by giving teams a preassembled workflow instead of starting from scratch. |
| **Boot disk image** | A prebuilt disk template used to start a virtual machine with a chosen operating system and software stack. | Like buying a laptop with the operating system and core apps already installed. | Cuts setup time and helps standardize environments across teams. |

## C

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **CLI** | Command-Line Interface: a text-based way to create, inspect, and manage cloud resources. | Like giving precise instructions at a drive-through speaker instead of tapping buttons on a kiosk. | Useful for automation, scripting, repeatability, and fast power-user workflows. |
| **Cluster** | A group of connected compute resources that work together as one system. | Like a team of workers assigned to one big project instead of one person doing it all. | Enables scale, resilience, and parallel processing for demanding AI jobs. |
| **Container** | A lightweight package that includes an application and the software it needs to run consistently across environments. | Like packing a food order in a sealed box with everything needed inside. | Improves portability, consistency, and deployment speed. |
| **Containerized application** | An application packaged and run inside a container. | Like shipping a mobile coffee stand that arrives with the espresso machine and supplies already inside. | Makes software easier to move between laptops, servers, and cloud platforms. |
| **Controller node** | In a Slurm/Soperator setup, the node that manages scheduling and orchestration of jobs. | Like an air traffic controller directing planes to the right runways and gates. | Coordinates work so jobs start in the right place at the right time. |
| **CUDA** | NVIDIA's parallel computing platform and programming model for running workloads on GPUs. | Like giving chefs a special kitchen layout so they can cook many dishes at once very efficiently. | Lets developers accelerate training, inference, and scientific computing on NVIDIA GPUs. |

## D

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Data preprocessing** | Cleaning, transforming, and organizing raw data before using it for training or inference. | Like washing, peeling, and chopping ingredients before cooking. | Improves model accuracy and reliability by feeding cleaner input into the pipeline. |
| **Device plugin** | A Kubernetes component that exposes specialized hardware, such as GPUs, to workloads running in the cluster. | Like a valet system that tells guests which specialty vehicles are actually available. | Allows containers to use scarce hardware resources in a controlled way. |
| **Distributed training** | Training a model across multiple GPUs or machines working together. | Like several construction crews building different parts of the same stadium at the same time. | Shortens training time for large models and datasets. |
| **Docker** | A widely used container platform for building and packaging containerized applications. | Like a standard brand of shipping container that works on many trucks, ships, and ports. | Makes application packaging and deployment more predictable. |

## E

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Endpoint** | In Serverless AI, an interactive service that listens for requests and returns model responses until stopped. | Like a staffed service desk that stays open to answer incoming questions. | Supports real-time AI experiences such as chat, search, and live predictions. |

## F

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Fault tolerance** | The ability of a system to keep operating even when some parts fail. | Like a restaurant staying open because another cook can step in when one calls out sick. | Improves uptime and user trust by reducing outages. |
| **Fine-tuning** | Adapting a pre-trained model to a narrower task or dataset by continuing training on new examples. | Like taking a general athlete and coaching them for one specific sport. | Improves relevance and quality for a company's specific use case. |
| **Framework** | A reusable software foundation that provides structure and common components for building applications. | Like the frame of a house that gives builders a standard structure to work with. | Speeds development and reduces custom reinvention. |

## G

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **GenAI** | Generative AI: systems that create new content such as text, images, code, or audio. | Like a creative assistant that drafts new material instead of only retrieving old files. | Enables products like copilots, chatbots, content tools, and design assistants. |
| **GlusterFS** | A distributed file system referenced by Nebius solution examples for shared storage across cluster nodes. | Like a shared company filing room that many teams can access from different offices. | Helps multiple machines read and write shared data needed by training jobs. |
| **GPU** | Graphics Processing Unit: a processor built to handle many calculations in parallel, making it well suited for AI workloads. | Like having hundreds of prep cooks working at once instead of one chef doing everything. | Accelerates training, inference, and data processing workloads that would be too slow on general-purpose chips. |
| **GPU cluster** | A cluster of machines or nodes equipped with GPUs and connected to work together on heavy workloads. | Like a fleet of tow trucks working the same major recovery job. | Provides the scale needed for large model training and high-throughput inference. |
| **GPU driver** | System software that lets the operating system and applications communicate correctly with the GPU. | Like the translator between the driver and a very specialized race car. | Required to make GPU hardware usable and stable for AI workloads. |
| **Grafana** | A visualization tool often used for dashboards that display metrics and system health. | Like a control-room wall of gauges and screens showing how the factory is running. | Helps teams monitor performance, spot anomalies, and troubleshoot faster. |

## H

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **High availability** | A design goal in which services are built to remain accessible with minimal downtime. | Like keeping a spare generator ready so the lights stay on when the power fails. | Protects revenue and operations by reducing service interruption. |
| **HPC** | High-Performance Computing: the use of powerful, often parallel systems to solve compute-intensive problems. | Like using an industrial bakery instead of a home oven when you need ten thousand loaves. | Supports large simulations, scientific workloads, and massive model training runs. |

## I

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Inference** | Using a trained model to generate predictions or outputs from new input data. | Like asking an experienced mechanic to identify a problem after years of training. | Turns trained models into usable products and business decisions. |
| **InfiniBand** | A high-throughput, low-latency networking technology used to connect systems for demanding compute workloads. | Like replacing neighborhood roads with a private high-speed express lane between factories. | Helps large GPU workloads exchange data faster, improving multi-node performance. |
| **Interactive workload** | A workload that stays running and responds to incoming requests in real time. | Like a help desk agent who stays at the phone waiting for calls. | Supports user-facing services where fast response matters. |

## J

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Job allocation** | The set of compute resources reserved by Slurm for a submitted job. | Like booking a meeting room, projector, and staff before an event starts. | Ensures the required resources are ready before the job runs. |
| **Job scheduler** | Software that decides when and where compute jobs should run based on rules and available resources. | Like a dispatcher assigning delivery routes to available drivers. | Improves utilization, fairness, and throughput in shared compute environments. |

## K

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **kubectl** | The native command-line tool used to work with Kubernetes clusters. | Like the remote control for a very large machine room. | Lets engineers inspect, update, and troubleshoot Kubernetes resources efficiently. |
| **Kubernetes** | An orchestration platform for deploying, scaling, and managing containerized applications. | Like an operations manager who decides where each shipping container goes and replaces broken trucks automatically. | Helps companies run AI and application workloads reliably at scale. |

## L

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Llama** | A family of large language models referenced in Nebius fine-tuning examples. | Like a pre-trained writer you can coach for your specific brand voice. | Serves as a base model for custom AI assistants and other language applications. |
| **Login node** | In a Slurm cluster, a node that users access to submit jobs and work with the environment. | Like the front desk and lobby where visitors arrive before going deeper into the building. | Provides a controlled entry point for users and workflows. |
| **LogQL** | A query language used for searching and analyzing logs in Loki-style systems. | Like a detective's search grammar for finding the right clues in a mountain of notes. | Helps teams quickly find errors, patterns, and operational signals in logs. |
| **Loki** | A log aggregation system often used alongside Grafana for storing and querying logs. | Like a searchable archive room for every machine and app message in the building. | Makes it easier to investigate incidents and understand system behavior. |

## M

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Managed Kubernetes** | Nebius's managed service for deploying and operating Kubernetes clusters with less manual overhead. | Like renting a serviced office where building management handles the plumbing and power. | Lets teams focus on applications instead of running every part of the cluster themselves. |
| **ML/AI workload** | A computing task related to machine learning or AI, such as training, inference, preprocessing, or evaluation. | Like the collection of jobs in a movie studio: filming, editing, sound, and release. | Helps teams categorize and optimize the kinds of compute work they run. |
| **MLflow** | An open-source platform for managing machine learning experiments and model lifecycle tasks. | Like a lab notebook mixed with a project tracker for model work. | Improves experiment tracking, reproducibility, and collaboration. |
| **Model evaluation** | Testing a model to measure how well it performs on defined tasks or datasets. | Like giving a student a final exam after months of study. | Prevents weak models from reaching customers and supports governance. |
| **Monitoring** | Collecting and viewing metrics, events, and health data about infrastructure and applications. | Like checking vital signs on a hospital monitor. | Helps teams detect issues early and keep services reliable. |
| **Multi-host training** | Training that spans multiple machines rather than a single server. | Like splitting a giant warehouse order across several fulfillment centers. | Needed when one machine does not have enough compute or memory for the job. |
| **Multi-node workload** | A job that runs across multiple nodes in a cluster. | Like a film production spread across several stages but following one production plan. | Allows larger or faster processing than a single node can provide. |

## N

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Node** | A single machine or compute instance that participates in a cluster. | Like one employee on a larger team. | Serves as a building block for scalable systems. |
| **Node group** | A set of similar nodes managed together inside a Kubernetes cluster. | Like a department made up of employees with the same role and equipment. | Makes it easier to scale and manage groups of machines consistently. |
| **NVLink** | NVIDIA's high-speed interconnect for moving data efficiently between GPUs. | Like a private hallway between offices instead of sending everything through the public street. | Improves performance when multiple GPUs need to share data rapidly. |

## O

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Observability** | The practice of understanding system health by using metrics, logs, traces, and related signals. | Like not just checking that a car is on, but also having the dashboard, service log, and engine diagnostics. | Speeds troubleshooting and improves operational reliability. |
| **Operator** | In Kubernetes, software that automates the deployment and lifecycle management of complex applications. | Like a specialist caretaker who knows how to install, tune, heal, and upgrade a specific machine. | Reduces manual administration and enforces best practices. |
| **Orchestration** | Coordinating many compute resources and workloads so they run in the right place and order. | Like a conductor keeping an orchestra in sync. | Essential for scaling AI systems efficiently and reliably. |

## P

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Parallel computing** | Using many processors or cores at the same time to solve parts of a problem together. | Like having many people assemble different sections of the same puzzle simultaneously. | Cuts runtime for large workloads and makes advanced AI feasible. |
| **Pod** | The basic deployable unit in Kubernetes that runs one or more tightly coupled containers. | Like a small work booth that can hold one specialist or a tiny team that must travel together. | Provides a practical unit for scheduling, scaling, and managing applications. |
| **PostgreSQL** | An open-source relational database system. | Like a very organized digital filing cabinet with strong rules for storing and finding records. | Supports applications that need reliable structured data storage. |
| **Project** | In Nebius, a resource boundary used to organize and control related cloud resources. | Like a labeled folder that keeps one department's budget, assets, and paperwork together. | Helps with organization, access control, and billing separation. |
| **Prometheus** | A monitoring system that collects and stores metrics from infrastructure and applications. | Like an automated clipboard that records performance readings at regular intervals. | Gives teams the data needed for dashboards, alerting, and capacity planning. |
| **Provisioning** | Creating and configuring infrastructure resources so they are ready to use. | Like setting up desks, laptops, and badges before a new team arrives. | Speeds onboarding of systems and supports automation. |

## Q

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Queue depth** | The number of requests or tasks waiting to be processed. | Like the number of people lined up at a coffee shop. | A useful signal for scaling systems and detecting bottlenecks. |

## R

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Real-time inference** | Producing model outputs immediately in response to live requests. | Like a translator speaking right as someone talks. | Important for chatbots, fraud checks, recommendations, and interactive apps. |
| **Region** | A geographic cloud location where resources run. | Like choosing which city to open a branch office in. | Affects latency, compliance, disaster planning, and service availability. |

## S

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Sbatch** | A Slurm command used to submit a batch script for execution. | Like handing a completed work order to the dispatcher. | Standardizes how jobs are submitted to the scheduler. |
| **Scheduling** | The process of assigning jobs to available resources over time. | Like deciding which meeting gets which room and when. | Keeps shared infrastructure efficient and fair. |
| **Serverless AI** | Nebius's service model for running AI endpoints or jobs without managing the underlying servers directly. | Like catering a meal without renting and staffing the kitchen yourself. | Speeds delivery and reduces operational overhead for AI teams. |
| **Service account** | A non-human identity used by applications or automation to access cloud resources. | Like a company badge issued to a robot worker instead of a person. | Improves security and automation by separating app permissions from user accounts. |
| **Shared filesystem** | A storage system that multiple machines can access as a common file space. | Like a shared drive everyone on a team can open. | Important for training data, checkpoints, and collaboration across nodes. |
| **Shared responsibility model** | A cloud security principle where the provider secures some layers and the customer secures others. | Like a landlord handling the building structure while the tenant locks their own office. | Clarifies who is responsible for security, compliance, and operations. |
| **Slurm** | An open-source workload manager and job scheduler widely used for high-performance computing and AI training. | Like a factory foreman assigning heavy jobs to the right crews and machines. | Helps organizations run large batch and training workloads efficiently. |
| **Soperator** | Nebius's open-source Kubernetes operator that runs Slurm nodes as Kubernetes Pods, combining Slurm and Kubernetes in one infrastructure. | Like mounting a factory foreman inside a modern operations control center so both work together. | Brings familiar Slurm job workflows to Kubernetes-based infrastructure. |
| **Srun** | A Slurm command used to launch tasks or job steps inside an allocated job. | Like telling individual crew members to start their part of the work after the site is reserved. | Supports multi-step and multi-node execution inside scheduled jobs. |

## T

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Terraform** | An infrastructure-as-code tool used to define and provision cloud resources from configuration files. | Like an architect's blueprint that can automatically assemble the building crew's work orders. | Improves repeatability, version control, and automation for infrastructure. |
| **Training** | The process of teaching a model by adjusting it using data so it can perform a task. | Like coaching a new employee through many examples until they get good at the job. | Creates the model capability that later powers AI products. |

## V

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Virtual machine (VM)** | A software-defined computer that runs its own operating system on shared physical hardware. | Like renting an apartment in a larger building: it feels like your own place even though the structure is shared. | Provides flexible isolated compute for apps, data jobs, and AI workloads. |

## W

| Term | Official definition | Easy analogy | Business purpose |
|---|---|---|---|
| **Worker node** | A node that actually runs application workloads or Slurm jobs. | Like the production floor where the real manufacturing happens. | Provides the compute capacity that does the work. |
| **Workflow** | An ordered sequence of steps that together complete a task or process. | Like a recipe with stages from prep to cooking to plating. | Helps teams standardize complex AI and data operations. |
| **Workload manager** | Software category that manages compute jobs and resource usage; Nebius discusses Slurm and Kubernetes in this role. | Like a dispatcher coordinating people, rooms, and equipment for many projects. | Improves utilization, scheduling, and operational control in shared environments. |
