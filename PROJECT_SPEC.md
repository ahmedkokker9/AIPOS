# 🤖 AIPOS Project Specification

> Version: 0.1.0 (Draft)

---

# 1. Introduction

## What is AIPOS?

AIPOS (AI Project Operating System) is an open-source framework designed to help AI coding agents develop software projects consistently, accurately, and efficiently.

Instead of relying solely on prompts or temporary conversation history, AIPOS provides a structured project specification that serves as a persistent source of truth throughout the entire software development lifecycle.

The framework is AI-agnostic and is designed to work with any AI coding agent, including current and future models.

---

## Why AIPOS Exists

Modern AI coding agents are capable of writing high-quality code, but they often struggle with long-term project consistency.

Common problems include:

- Forgetting previous architectural decisions.
- Duplicating existing logic.
- Breaking established project conventions.
- Losing awareness of the current project state.
- Producing inconsistent implementations across multiple sessions.

AIPOS addresses these challenges by maintaining structured project knowledge that remains available across the entire development lifecycle.

---

## Vision

Enable AI coding agents to work as reliable software engineering partners rather than simple code generators.

The ultimate goal is to make AI-assisted software development predictable, maintainable, scalable, and production-ready.

---

## Core Objectives

The framework is designed around the following objectives:

- Maintain long-term project context.
- Preserve architectural consistency.
- Standardize development workflows.
- Reduce repetitive prompting.
- Improve collaboration between humans and AI agents.
- Support any AI coding platform.
- Produce production-ready software by default.

---

## Design Principles

Every decision in AIPOS follows these principles:

### 1. AI First

The framework is designed primarily for AI agents while remaining understandable for human developers.

---

### 2. Single Source of Truth

Every piece of information should exist in one place only.

Avoid duplicated documentation.

---

### 3. Production Ready

Generated software should follow modern engineering practices.

Shortcuts are discouraged.

---

### 4. Consistency Over Creativity

Consistency produces maintainable software.

Whenever multiple valid solutions exist, prefer the solution that keeps the project consistent.

---

### 5. Framework Agnostic

AIPOS does not depend on a specific programming language, framework, or technology stack.

---

### 6. AI Agnostic

AIPOS must work equally well with any AI coding agent without requiring vendor-specific behavior.

---

### 7. Living Documentation

The project specification evolves together with the project.

Documentation is continuously refined instead of becoming outdated.

---

## Non Goals

AIPOS is not:

- A code generator.
- A prompt library.
- A boilerplate project.
- A replacement for software architecture.
- A replacement for engineering judgment.

Instead, it provides structure that helps AI agents produce better software.

---

# 2. AI Execution Model

## Purpose

This chapter defines how any AI coding agent should interact with a project that uses AIPOS.

The goal is to ensure that every AI agent follows the same engineering process, regardless of the underlying model or platform.

This execution model is AI-agnostic and applies equally to all supported AI coding agents.

---

## Responsibilities

An AI agent working with AIPOS is expected to:

- Understand the project before making changes.
- Preserve architectural consistency.
- Avoid duplicated implementations.
- Complete one task before starting another.
- Keep documentation synchronized with the project.
- Produce production-ready code instead of prototypes whenever possible.

---

## Core Principles

Every action performed by an AI agent should follow these principles.

### Understand Before Acting

Never modify code before understanding the current implementation.

Always inspect existing files before creating new ones.

---

### Reuse Before Creating

Always prefer extending existing implementations.

Avoid introducing duplicate logic, duplicate utilities, or duplicate components.

---

### Consistency Over Preference

Follow the existing project conventions.

Do not introduce a different coding style or architectural pattern unless explicitly requested.

---

### Finish Before Switching

Complete the current task before moving to another one.

Avoid leaving partially implemented features.

---

### Documentation Stays in Sync

Whenever a change affects the project specification, documentation should be updated accordingly.

Documentation should reflect the current state of the project.

---

## Standard Execution Cycle

Every implementation should follow this sequence.

1. Understand the request.

2. Analyze the existing project.

3. Create an implementation plan.

4. Implement the solution.

5. Validate the implementation.

6. Review the result.

7. Update project documentation if necessary.

8. Mark the task as complete.

Never skip validation.

---

## General Rules

The AI agent should:

- Write clean and maintainable code.
- Respect project architecture.
- Keep implementations simple.
- Prefer readability over cleverness.
- Avoid unnecessary abstractions.
- Minimize technical debt.
- Consider security and performance when appropriate.

---

## Things the AI Must Never Do

Never:

- Remove existing functionality without explicit instruction.
- Rewrite large parts of the project unnecessarily.
- Duplicate existing logic.
- Ignore project conventions.
- Invent undocumented requirements.
- Leave unfinished implementations.
- Expose secrets or sensitive information.

---

## Definition of Success

A task is considered complete only if:

- The requested functionality is implemented.
- The implementation follows project standards.
- Existing functionality is preserved.
- No unnecessary complexity is introduced.
- Documentation is updated when required.

# 3. Context Management

## Purpose

Context is the foundation of every successful AI-assisted software project.

Unlike human developers, AI agents rely entirely on the information available during each interaction. Missing or inconsistent context often leads to incorrect implementations, duplicated logic, and architectural inconsistencies.

AIPOS provides a structured approach to managing project context, ensuring that AI agents always have access to the information required to make consistent engineering decisions.

---

## Context Philosophy

Every AI decision should be based on explicit project context rather than assumptions.

Whenever required information is unavailable, the AI should request clarification instead of making undocumented decisions.

Reliable context produces reliable software.

---

## Types of Context

AIPOS organizes project knowledge into multiple context categories.

Each category has a specific purpose and should remain independent.

### Project Context

Defines the project's overall purpose.

Includes:

- Project vision
- Business goals
- Scope
- Technology stack

This context changes infrequently.

---

### Architecture Context

Defines how the software is structured.

Includes:

- Architecture
- Module boundaries
- Design patterns
- Folder organization

Architectural consistency should always be preserved.

---

### Task Context

Represents the current work being performed.

Includes:

- Current objective
- Requirements
- Dependencies
- Acceptance criteria

Task context is temporary.

---

### Decision Context

Stores important engineering decisions made throughout the project.

Examples include:

- Technology selection
- Architectural changes
- Design trade-offs

Decisions should remain traceable.

---

### Progress Context

Represents the current state of the project.

Includes:

- Completed work
- Current milestone
- Active tasks
- Known blockers

This context evolves continuously.

---

### Historical Context

Captures previous implementations and project evolution.

Historical context allows future AI agents to understand why the project reached its current state.

---

## Context Loading Strategy

AI agents should load only the context required for the current task.

Avoid unnecessary information that does not contribute to the implementation.

Loading relevant context improves consistency while reducing cognitive overhead.

---

## Context Priority

When multiple sources of information exist, they should be considered in the following order:

1. Explicit user instructions.
2. Current project specification.
3. Existing project implementation.
4. Previous engineering decisions.
5. General engineering best practices.

Never allow assumptions to override explicit project requirements.

---

## Context Integrity

Project context should always remain:

- Accurate
- Consistent
- Up to date
- Non-duplicated
- Traceable

Every important change should be reflected in the appropriate project documentation.

---

## Context Boundaries

Different context types should not be mixed unnecessarily.

For example:

- Architecture should not describe coding style.
- Progress should not redefine project goals.
- Historical decisions should not replace current requirements.

Each context should have a single responsibility.

---

## Missing Context

When required context is unavailable, AI agents should:

1. Search the existing project.
2. Review the project specification.
3. Ask for clarification if necessary.

Never invent project requirements.

---

## Context Quality Checklist

A well-maintained project context should be:

- Complete
- Consistent
- Up to date
- Easy to understand
- Free from duplication
- Structured
- Actionable
- Relevant

Poor context leads to poor software.

---

## Key Principle

AI agents should rely on structured project context rather than temporary conversation history whenever possible.

AIPOS exists to make project knowledge persistent, reliable, and reusable across the entire software development lifecycle.

# 3. Context Management

## Purpose

Context is the foundation of every successful AI-assisted software project.

Unlike human developers, AI agents rely entirely on the information available during each interaction. Missing or inconsistent context often leads to incorrect implementations, duplicated logic, and architectural inconsistencies.

AIPOS provides a structured approach to managing project context, ensuring that AI agents always have access to the information required to make consistent engineering decisions.

---

## Context Philosophy

Every AI decision should be based on explicit project context rather than assumptions.

Whenever required information is unavailable, the AI should request clarification instead of making undocumented decisions.

Reliable context produces reliable software.

---

## Types of Context

AIPOS organizes project knowledge into multiple context categories.

Each category has a specific purpose and should remain independent.

### Project Context

Defines the project's overall purpose.

Includes:

- Project vision
- Business goals
- Scope
- Technology stack

This context changes infrequently.

---

### Architecture Context

Defines how the software is structured.

Includes:

- Architecture
- Module boundaries
- Design patterns
- Folder organization

Architectural consistency should always be preserved.

---

### Task Context

Represents the current work being performed.

Includes:

- Current objective
- Requirements
- Dependencies
- Acceptance criteria

Task context is temporary.

---

### Decision Context

Stores important engineering decisions made throughout the project.

Examples include:

- Technology selection
- Architectural changes
- Design trade-offs

Decisions should remain traceable.

---

### Progress Context

Represents the current state of the project.

Includes:

- Completed work
- Current milestone
- Active tasks
- Known blockers

This context evolves continuously.

---

### Historical Context

Captures previous implementations and project evolution.

Historical context allows future AI agents to understand why the project reached its current state.

---

## Context Loading Strategy

AI agents should load only the context required for the current task.

Avoid unnecessary information that does not contribute to the implementation.

Loading relevant context improves consistency while reducing cognitive overhead.

---

## Context Priority

When multiple sources of information exist, they should be considered in the following order:

1. Explicit user instructions.
2. Current project specification.
3. Existing project implementation.
4. Previous engineering decisions.
5. General engineering best practices.

Never allow assumptions to override explicit project requirements.

---

## Context Integrity

Project context should always remain:

- Accurate
- Consistent
- Up to date
- Non-duplicated
- Traceable

Every important change should be reflected in the appropriate project documentation.

---

## Context Boundaries

Different context types should not be mixed unnecessarily.

For example:

- Architecture should not describe coding style.
- Progress should not redefine project goals.
- Historical decisions should not replace current requirements.

Each context should have a single responsibility.

---

## Missing Context

When required context is unavailable, AI agents should:

1. Search the existing project.
2. Review the project specification.
3. Ask for clarification if necessary.

Never invent project requirements.

---

## Context Quality Checklist

A well-maintained project context should be:

- Complete
- Consistent
- Up to date
- Easy to understand
- Free from duplication
- Structured
- Actionable
- Relevant

Poor context leads to poor software.

---

## Key Principle

AI agents should rely on structured project context rather than temporary conversation history whenever possible.

AIPOS exists to make project knowledge persistent, reliable, and reusable across the entire software development lifecycle.
# 5. Project Specification

## Purpose

Every software project requires a clear and consistent specification that defines what should be built, why it should be built, and how it should evolve over time.

AIPOS standardizes this specification to ensure that both AI agents and human developers work from the same source of truth throughout the entire project lifecycle.

The project specification should describe the project itself, not the implementation details of a single task.

---

## Core Principle

A project specification should answer every essential question an AI agent needs before writing code.

If important information is missing, it should be considered incomplete rather than inferred.

---

## Standard Specification Structure

Every AIPOS project specification should include the following sections.

### 1. Project Information

Provides a high-level overview of the project.

Includes:

- Project name
- Short description
- Project vision
- Target users
- Project scope

---

### 2. Business Objectives

Defines why the project exists.

Includes:

- Business goals
- User problems
- Expected outcomes
- Success criteria

Business objectives should remain independent from technical implementation.

---

### 3. Functional Requirements

Defines what the system must do.

Requirements should describe expected behavior rather than implementation.

Examples include:

- User authentication
- Product management
- Payment processing
- Notifications

---

### 4. Non-Functional Requirements

Defines system quality expectations.

Examples include:

- Performance
- Scalability
- Security
- Reliability
- Accessibility
- Maintainability

---

### 5. Technology Stack

Defines the technologies used within the project.

Examples include:

- Programming languages
- Frameworks
- Databases
- Infrastructure
- External services

Technology choices should be documented explicitly.

---

### 6. System Architecture

Describes how the software is organized.

Includes:

- Architectural style
- Project structure
- Major modules
- Service boundaries
- Data flow

Architecture should remain stable throughout the project lifecycle.

---

### 7. Development Standards

Defines engineering conventions followed by the project.

Examples include:

- Coding standards
- Naming conventions
- Folder organization
- Testing strategy
- Git workflow

Development standards promote consistency across contributors.

---

### 8. Project Context

Provides the information required to understand the current state of the project.

Includes:

- Active milestone
- Current progress
- Important decisions
- Known limitations
- Future plans

Project context should evolve continuously.

---

## Specification Characteristics

A high-quality project specification should be:

- Complete
- Accurate
- Consistent
- Structured
- Easy to navigate
- Maintainable
- Free from duplication

---

## Specification Ownership

The project specification is the primary source of truth.

Whenever conflicts exist between undocumented assumptions and the specification, the specification takes precedence.

All significant project changes should eventually be reflected in the specification.

---

## Specification Maintenance

The specification should evolve alongside the software.

Outdated documentation reduces implementation quality and should be updated whenever major project changes occur.

Documentation is part of the project, not an optional artifact.

---

## Key Principle

The project specification defines the knowledge required to build the project successfully.

High-quality software begins with high-quality project knowledge.