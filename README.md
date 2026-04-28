[![MseeP.ai Security Assessment Badge](https://mseep.net/pr/asultani91-amazon-bedrock-agentcore-with-strands-agents-nova-pro-badge.png)](https://mseep.ai/app/asultani91-amazon-bedrock-agentcore-with-strands-agents-nova-pro)

# 🤖 Amazon Bedrock AgentCore Workshop with Strands Agents & Nova Pro

A comprehensive hands-on workshop demonstrating production-ready infrastructure for Agentic AI using **Amazon Bedrock AgentCore**, **Strands Agents framework**, and **Amazon Nova Pro** foundation model. This project covers seven modular labs that progressively build expertise in deploying secure, scalable AI agents at enterprise scale.

> **Workshop Repository:** [aws-samples/sample-bedrock-agentcore-with-strands-and-nova](https://github.com/aws-samples/sample-bedrock-agentcore-with-strands-and-nova/)
> **Target Audience:** Solution Architects, Software Designers, Developers
> **Duration:** Multi-day workshop (7 labs)
> **Supported Regions:** us-east-1, us-west-2, eu-central-1, ap-southeast-2

---

## 🎯 Project Overview

This workshop demonstrates how to build production-ready AI agents using AWS's comprehensive AgentCore platform. Unlike basic chatbots, these agents can:

- ✅ Execute Python code in isolated environments
- ✅ Automate web browser interactions
- ✅ Securely manage API credentials
- ✅ Remember conversations across sessions
- ✅ Access external APIs through standardized protocols
- ✅ Provide full observability and debugging capabilities

---

## 🏗️ What is Amazon Bedrock AgentCore?

**Amazon Bedrock AgentCore** is a comprehensive platform that enables deployment and operation of highly effective AI agents securely at scale.

### Key Features:
- **Framework Flexibility:** Works with any agent framework (CrewAI, LangGraph, LlamaIndex, Strands Agents)
- **Model Agnostic:** Supports any foundation model inside or outside Amazon Bedrock
- **Purpose-Built Infrastructure:** Optimized for dynamic agent workloads
- **Production Controls:** Essential security and governance for real-world deployment

### AgentCore Modular Services

| Service | Purpose |
|---------|---------|
| **AgentCore Runtime** | Low-latency serverless environments with session isolation, supporting any framework and long-running agents (up to 8 hours) |
| **AgentCore Memory** | Manages session and long-term memory, providing context while agents learn from past interactions |
| **AgentCore Identity** | Enables secure access to AWS services and third-party tools (GitHub, Salesforce, Slack) with user consent |
| **AgentCore Gateway** | Transforms APIs and Lambda functions into agent-ready tools with unified MCP protocol access |
| **AgentCore Code Interpreter** | Isolated environment to execute agent-generated code in Python, JavaScript, TypeScript |
| **AgentCore Browser** | Managed web browser instances for web automation workflows |
| **AgentCore Observability** | Step-by-step visualization with metadata tagging, scoring, trajectory inspection, and debugging |

---

## 🧵 What is Strands Agents?

**Strands Agents** is a code-first framework for building and running AI agents in just a few lines of code.

### Key Features:
- ✅ **Lightweight & Customizable:** Simple agent loop that's fully extensible
- ✅ **Production Ready:** Full observability, tracing, and deployment options
- ✅ **Model Agnostic:** Supports multiple models from various providers
- ✅ **Community Tools:** Quick start with powerful contributed tools
- ✅ **Multi-Agent Support:** Agent teams and autonomous self-improving agents
- ✅ **Flexible Modes:** Conversational, non-conversational, streaming, non-streaming
- ✅ **Security First:** Responsible agent operation with data protection

---

## 🚀 What is Amazon Nova Pro?

**Amazon Nova Pro** is Amazon's highly capable, multimodal generative AI foundation model that excels at:

- 📝 **Text Processing:** Advanced language understanding and generation
- 🖼️ **Image Analysis:** Deep visual understanding and processing
- 🎥 **Video Processing:** Multimodal video analysis capabilities
- 📊 **Document Analysis:** Complex document understanding
- 📈 **Data Visualization:** Deep analytical capabilities

**Access:** Available through Amazon Bedrock with strong balance of accuracy, speed, and cost.

---

## 🧪 Workshop Labs

### **Lab 0: Getting Started with Strands Agents**
Foundation lab to familiarize with Strands Agents framework.

**Key Learnings:**
- Build agents with tools in few lines of code
- Run agents locally with Nova Pro as the brain
- Create custom tools for specific use cases
- Explore conversation history and agent memory

---

### **Lab 1: AgentCore Code Interpreter** 🧮

**Objective:** Integrate Strands Agents with AgentCore Code Interpreter for dynamic Python code execution.

**What I Built:**
- Default sandboxed Code Interpreter for math operations
- Custom Code Interpreter with public network access
- Stock price retrieval using external APIs

**Key Concepts:**
- Secure code execution in containerized environments
- Support for Python, JavaScript, TypeScript
- File references from Amazon S3 for large datasets
- Extended execution time (15 minutes default, up to 8 hours)
- Structured data handling (CSV, Excel, JSON)

**Use Cases:**
- Data analysis and cleaning
- Mathematical calculations at scale
- Multi-step computational problem solving

---

### **Lab 2: AgentCore Browser** 🌐

**Objective:** Build AI agents capable of web automation using AgentCore Browser.

**What I Built:**
- Direct browser session access using Playwright
- Autonomous web navigation agents
- Element interaction (click, extract, summarize)
- AWS Builder Center content extraction

**Key Concepts:**
- Secure, isolated browser environments
- Visual understanding through screenshots
- Session isolation and audit capabilities
- Human intervention with live interactive view

**Use Cases:**
- Web application testing
- Form submissions and data entry
- Information extraction from websites
- E-commerce transactions
- Website monitoring and updates

---

### **Lab 3: AgentCore Identity for API Key Security** 🔐

**Objective:** Securely manage API keys and credentials for external services.

**What I Built:**
- Secure API Key Credential Providers
- Exa Search API integration with proper credential management
- Elimination of hardcoded credentials

**Key Concepts:**
- Centralized credential management
- AWS IAM (SigV4) authentication
- OAuth 2.0 integration
- API key secure storage
- Independent request verification

**Security Benefits:**
- No credential exposure in code
- Audit trails for all access attempts
- Integration with corporate identity providers (Okta, Microsoft Entra ID, Amazon Cognito)

---

### **Lab 4: AgentCore Runtime for MCP Server Deployment** 📦

**Objective:** Deploy Model Context Protocol (MCP) servers to AgentCore Runtime as managed services.

**What I Built:**
- Custom MCP server with web search functionality
- Amazon Cognito authentication setup
- Cloud-native MCP server deployment
- Local Strands Agent integration with deployed MCP server

**Key Concepts:**
- **Framework Agnostic:** Works with LangGraph, Strands, CrewAI
- **Model Flexibility:** Any LLM (Bedrock, Claude, Gemini, OpenAI)
- **MCP Protocol Support:** Standardized tool communication
- **Extended Execution:** Up to 8 hours for complex reasoning
- **Session Isolation:** Dedicated microVM per user session
- **Consumption-Based Pricing:** Pay only for resources consumed

---

### **Lab 5: AgentCore Runtime with Observability** 📊

**Objective:** Deploy Strands Agents with comprehensive monitoring and debugging capabilities.

**What I Built:**
- Strands Agent with weather and calculator tools
- AgentCore Runtime deployment with boto3/IAM
- CloudWatch integration for GenAI observability
- Session management and isolation testing

**Key Concepts:**
- **Built-in Tracing:** Captures reasoning steps, tool invocations, model interactions
- **OpenTelemetry (OTEL) Compatible:** Integrates with existing monitoring stacks
- **GenAI Semantic Conventions:** Framework-aware instrumentation
- **Real-Time Dashboards:** Session count, latency, token usage, error rates
- **Rich Metadata:** Tagging, filtering, custom scoring

**Observability Features:**
- Step-by-step execution visualization
- Trajectory inspection for debugging
- Performance bottleneck identification
- Quality maintenance at scale

---

### **Lab 6: AgentCore Memory (Short-Term & Long-Term)** 🧠

**Objective:** Create agents with persistent memory across conversations and sessions.

**What I Built:**
- Short-term memory for immediate context
- Long-term memory for user preferences
- Memory-enabled personalized agent experiences
- Context retention across sessions

**Memory Types:**

#### Short-Term Memory
- Stores raw interactions within a single session
- Operations: `CreateEvent`, `ListSessions`, `ListEvents`, `GetEvent`
- Maintains conversation context

#### Long-Term Memory
- Stores structured insights extracted from conversations
- **Asynchronous Extraction:** Background processing without interrupting interactions
- **Consolidation:** Merges new information with existing knowledge
- Operations: `CreateMemory`, `GetMemoryRecord`, `ListMemoryRecords`, `RetrieveMemoryRecords`

**Benefits:**
- Personalized user experiences
- Context-aware responses
- Reduced redundant questions
- Learning from past interactions

---

### **Lab 7: AgentCore Gateway for OpenAPI to MCP Transformation** 🔌

**Objective:** Automatically generate MCP servers from OpenAPI specifications.

**What I Built:**
- AgentCore Gateway with authentication
- OpenAPI-based gateway targets (Exa Search API)
- Secure credential management for external APIs
- Strands Agent integration with gateway

**Key Concepts:**
- **Transform Existing APIs:** Convert REST APIs to agent-ready tools without custom code
- **Unified Access:** Single endpoint for multiple tool sources
- **Comprehensive Authentication:** Inbound (IAM/OAuth) and outbound (OAuth/API keys)
- **Semantic Search:** Contextual tool discovery at scale
- **1-Click Integrations:** Salesforce, Slack, Jira, Asana, Zendesk

**Gateway Target Types:**
- **OpenAPI:** RESTful services with OpenAPI schemas
- **Smithy:** AWS service definitions
- **Lambda:** AWS Lambda functions

---

## 🛠️ Technologies Used

### AWS Services
- **Amazon Bedrock** – Foundation model hosting
- **Amazon Bedrock AgentCore** – All 7 modular services
- **AWS Lambda** – Serverless compute
- **Amazon CloudWatch** – Observability and monitoring
- **Amazon ECR** – Container registry
- **Amazon Cognito** – User authentication
- **Amazon S3** – Data storage
- **AWS IAM** – Identity and access management
- **AWS CloudFormation** – Infrastructure as code

### Frameworks & Languages
- **Strands Agents** – AI agent framework
- **Python 3.11** – Primary language
- **Jupyter Notebook** – Interactive development
- **OpenTelemetry (OTEL)** – Observability instrumentation
- **Playwright** – Browser automation
- **Docker** – Containerization

### AI Models
- **Amazon Nova Pro** – Multimodal foundation model
- **Model Context Protocol (MCP)** – Tool communication standard

### Development Tools
- **Visual Studio Code** – IDE
- **uv** – Python environment manager
- **boto3** – AWS SDK for Python
- **ADOT** – AWS Distro for OpenTelemetry

---

## 📐 Architecture Highlights

The workshop includes comprehensive architecture diagrams for:

1. **AgentCore Code Interpreter** – Isolated code execution flow
2. **AgentCore Browser** – Web automation with visual feedback
3. **AgentCore Identity** – Multi-path authentication architecture
4. **AgentCore Runtime (MCP)** – Containerized MCP server deployment
5. **AgentCore Runtime (Agent)** – Framework deployment pipeline
6. **AgentCore Observability** – OTEL integration and dashboards
7. **AgentCore Memory** – Short-term and long-term memory systems
8. **AgentCore Gateway** – API transformation and tool management

All diagrams demonstrate clear data flow, security boundaries, and service interactions.

---

## 🎯 Key Learning Outcomes

By completing this workshop, I gained expertise in:

✅ **AgentCore Architecture** – Mastered all 7 modular services
✅ **Production Agent Deployment** – Moved from local to cloud-native deployments
✅ **Security Implementation** – Proper credential management and session isolation
✅ **Observability** – Full tracing and debugging capabilities
✅ **Agent Memory Management** – Short-term and long-term memory strategies
✅ **External Tool Integration** – MCP servers and OpenAPI transformations
✅ **Web Automation** – Browser automation with AI agents
✅ **Safe Code Execution** – Sandboxed code interpretation
✅ **Framework Flexibility** – Working with any agent framework or model
✅ **Scalable Architecture** – Consumption-based pricing and auto-scaling

---

## 📸 Screenshots & Diagrams

The project includes detailed screenshots from:
- AWS Bedrock Console (Model access configuration)
- CloudWatch Console (Transaction Search setup)
- CloudFormation Console (Code Editor stack)
- Visual Studio Code (Jupyter Notebook interface, kernel selection, code execution)
- Architecture diagrams for all 7 AgentCore services

All diagrams are stored in the `/images` folder with descriptive filenames.

---

## 🚀 Setup Instructions

### Prerequisites
- AWS Account with appropriate IAM permissions
- Python 3.11+
- Docker installed
- Basic knowledge of AWS services

### Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/aws-samples/sample-bedrock-agentcore-with-strands-and-nova
   cd sample-bedrock-agentcore-with-strands-and-nova
