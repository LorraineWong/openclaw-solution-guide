## 0. Core Value

> OpenClaw = Upgrading AI from a “chat tool” to an “execution system”

Its core capability can be summarized as:

> Understand → Decide → Execute

In practical terms, this means:

- Understand what you want
- Decide what to do
- Call system capabilities to complete the action

The key point: OpenClaw is not only for answering questions, but also for actually completing tasks.

---

## 1. Background

In many traditional systems, software stores data, but people still have to do the real work manually.

For example:
- Customer service manually checks order status
- Employees manually submit processes
- Managers wait for analysis from a data team

So the common pattern is:

> The system stores data, people execute tasks

Now, with large models, we can describe needs in natural language. But in many cases, AI is still only used for conversation, not real execution.

So the core problem is:

> **AI can understand, but cannot execute**

---

### 1.1 Solution Overview

OpenClaw’s goal is to turn language understanding into real execution.

Example: query order status.

| Mode | How it works | Limitation / Result |
|------|--------------|---------------------|
| Traditional | User → Customer service → Log in system → Query → Reply | Manual, slow |
| AI chat tool | User → AI → AI generates an answer | May not use real business data |
| OpenClaw | User → Agent → Call system API → Get real data → Return result | Can execute and return real results |

So the key is not “smarter replies,” but “whether actions can be executed.”

---

### 1.3 Positioning

OpenClaw is not just one model and not just one app.

It is:

> **An AI execution system that converts understanding into real actions**

---

## 2. How It Works (Simplified)

When you send a request, OpenClaw follows a clear path:

User request  
↓  
Gateway  
↓  
Agent  
↓  
Model  
↓  
Tools / Skills  
↓  
Return result

A simple understanding of the process:

> Request → Understand → Decide → Execute → Return

This is the core difference from pure chat systems.

---

## 3. Deployment and Usage

This section focuses on what individual users care about most: how to run it and use it quickly.

---

### 3.1 Environment Requirements

You can run OpenClaw on a personal computer or server.

Basic requirements:

- Installed Node.js (LTS recommended)
- Network access (for model access or dependency downloads)
- Open port if needed (default: `18789`)

---

### 3.2 Deployment and Startup

Install OpenClaw:

```bash
npm install -g openclaw
```

Initialize:

```bash
openclaw onboard --install-daemon
```

Start service:

```bash
openclaw gateway --port 18789
```

Open in browser:

```bash
http://localhost:18789
```

If running on a server, use the server IP and port.

---

### 3.3 Initialization and Basic Configuration

After startup, complete two basic steps:

1. Configure a model
   - Cloud models (for example: OpenAI, Claude)
   - Local models (for example: Qwen, DeepSeek)

2. Create an Agent
   - For example: “General Assistant” or “Customer Service Assistant”

After this, the system can handle basic interaction and start execution workflows.

---

### 3.4 Quick Start

Use this quick checklist:

1. Open the web interface
2. Confirm model is configured successfully
3. Create an Agent
4. Enter simple prompts, such as:
   - Hello
   - Help me summarize artificial intelligence

If the system returns results normally, deployment is successful.

---

### 3.5 Basic Usage Path

You can use OpenClaw step by step:

1. Start with normal conversation to verify it works
2. Add data/tools access so it can get real information
3. Let it execute concrete actions (for example, query or trigger a process)

This is a practical path from:

> “System available” → “Capability expanded” → “Practical use”

---

### 3.6 Deployment Modes

You can choose one mode based on your current stage:

**1) Single-machine experience (PoC)**
- Environment: personal computer / test server
- Use: quick trial and demo
- Feature: fast and low cost

**2) Department-level deployment**
- Environment: enterprise server / cloud host
- Use: specific scenario (for example, customer service, operations)
- Feature: supports multiple users and partial system access

**3) Enterprise-level deployment**
- Environment: private cloud / data center / all-in-one machine
- Use: deeper core-business integration
- Feature: broader access and stronger stability

---

### 3.7 Model Selection Suggestions

Choose models by scenario:

| Scenario | Recommended Model |
|------|-------------------|
| General conversation | GPT / Claude |
| Chinese business scenarios | Qwen / DeepSeek |
| Local deployment | Qwen local version |
| Cost-sensitive | Open-source models |

---

## 4. Practical Understanding of “Execution Capability”

Why OpenClaw is different:

- A model alone usually outputs text
- OpenClaw can decide whether to call tools and then execute actions

So in OpenClaw:

- You provide intent in natural language
- The system completes the operation

In short:

> Interaction is still conversation, but the result becomes task completion

---

## 5. Summary

OpenClaw’s core value is enabling AI to actually do tasks, not only reply with text.

The complete loop is:

- Understand the request
- Decide the path
- Execute the action
- Return the result

> From “AI available” to “AI executable”
