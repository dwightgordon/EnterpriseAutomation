# EnterpriseAutomation

## Overview

EnterpriseAutomation is a structured enterprise desktop foundation built with **WPF (.NET 8 LTS)** using modern .NET architectural principles.

This project focuses on building a clean, extensible platform using:

- MVVM architecture  
- Generic Host (Microsoft.Extensions.Hosting)  
- Dependency Injection  
- Layered application design  
- Clean separation of concerns  

The primary goal is to establish a stable desktop platform before expanding into orchestration, automation services, and potential backend integration.

---

## Architectural Principles

This project is built with the following engineering principles:

- Stability over preview tooling (.NET 8 LTS)
- Explicit dependency management
- Environment consistency
- Clean layering
- Reproducible builds
- Source-controlled configuration

The application lifecycle is managed via the .NET Generic Host, enabling:

- Centralized service registration
- Dependency injection container
- Application startup/shutdown control
- Future extensibility toward backend or API architectures

---

## Technology Stack

- .NET 8 (LTS)
- WPF
- Microsoft.Extensions.Hosting
- Microsoft.Extensions.DependencyInjection
- Git / GitHub version control

---

## Current Architecture

EnterpriseAutomation
│
├── EnterpriseAutomation.Desktop
│   ├── Views
│   ├── ViewModels
│   ├── Services
│   ├── App.xaml
│   └── App.xaml.cs

Key characteristics:

- No business logic in code-behind
- DI container bootstrapped via Generic Host
- MainWindow resolved through dependency injection
- Structured for future service abstraction

---

## Development Environment

- Visual Studio (stable channel)
- .NET 8 SDK
- Consistent SDK resolution (no preview dependency)

---

## Current Status

- Stable WPF foundation
- .NET 8 SDK enforced
- Generic Host configured
- Dependency Injection operational
- Repository baseline established
- Environment parity validated across machines

---

## Roadmap

Next architectural steps:

- Introduce MainViewModel
- Implement DataContext binding
- Introduce command infrastructure
- Expand service layer
- Implement structured logging
- Prepare for optional backend abstraction

---

## Long-Term Vision

EnterpriseAutomation is designed as a scalable foundation.

Future directions may include:

- Backend service layer (ASP.NET Core)
- Remote execution capabilities
- Centralized orchestration
- Multi-user architecture
- Persistence layer integration

The desktop platform is intentionally built with clean separation to allow this evolution without architectural rewrites.
