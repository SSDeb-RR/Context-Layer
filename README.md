# ContextLayer: Git/GitHub for AI Context

ContextLayer is a cloud-based system for storing, organizing, and versioning the context used inside AI applications. Instead of scattering prompts, rules, memory, and retrieved data across code and tools, ContextLayer lets you treat context as a first-class, versioned resource that lives in one place and evolves with your application. It brings software-style version control to AI context — complete with structured organization, history tracking, and programmable access.

🔗 **Live App:** https://get-context-layer.lovable.app/

## What ContextLayer Does

ContextLayer helps developers manage the context layer of AI systems — the system prompts, rules, memory, retrieved documents, and other structured inputs that shape model behavior. With ContextLayer, you can store context centrally in the cloud, organize context into logical Blocks, create multiple Versions of the same block, track a full change history (like commits), retrieve compiled context directly inside your code, and manage everything visually through a web dashboard. In short, it's Git for AI context.

## Core Concepts

**Project** represents one AI application or system. **Block** is a named container for related context. Examples include `support_faq`, `pricing_rules`, `assistant_personality`, and `rag.documents`. **Version** allows each block to have multiple versions — enabling different context timelines for experiments, staging versus production, and more. **History** means every change (add, update, delete) is recorded so you can see exactly how a block evolved over time.

## Use It From Code (SDK)

ContextLayer provides an SDK so developers can manage context directly from their applications.

```python
from contextlayer import CL

cl = CL(api_key="your_project_api_key")

cl.append("support_faq", "Refunds are allowed within 7 days.")
cl.append("assistant_personality", "Respond in a friendly but professional tone.")

context = cl.get("support_faq")
```

That same context is instantly visible in the cloud dashboard, along with its history and version information.

## Use It From the Cloud Dashboard

Everything you can do programmatically, you can also do visually: create and manage Projects, add or edit Blocks, switch between Versions, view compiled context, and explore full change history in a timeline view. This makes it easy to collaborate, audit changes, and understand how your AI system's behavior has evolved.

## Versioning for AI Behavior

ContextLayer isn't just storage — it's controlled evolution of AI context. You can create a new version of a block before trying a prompt change, compare how context differed over time, and roll forward with new behavior while preserving past states. This makes prompt and context engineering more like software development and less like guesswork.

## Why ContextLayer Exists

AI applications rely heavily on context — but today, that context is often hardcoded, duplicated across services, lost over time, and impossible to version properly. ContextLayer solves this by making context centralized, structured, versioned, and traceable. So AI systems can be built with the same rigor as traditional software.

## Who It's For

ContextLayer is built for AI engineers, prompt engineers, teams building LLM-powered applications, and anyone who wants reproducible, controllable AI behavior.

**ContextLayer = Git for AI context.**
