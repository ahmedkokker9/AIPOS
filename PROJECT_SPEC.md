
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
