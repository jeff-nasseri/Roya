# RoyaAI

RoyaAI is an advanced AGI (Artificial General Intelligence) platform that enables agents to interact with operating systems through a secure kernel architecture. This platform provides a structured and safe way for AI agents to perform file operations, access system information, and execute shell commands, all while maintaining proper security boundaries.

## Core Architecture

RoyaAI consists of several key components:

- **Kernel**: The system layer providing direct interaction with OS APIs that agents can call
- **Agent**: LLM models connected to the system, serving as the main intelligence of the platform
- **Node**: Dedicated machines where agents can access and operate through the kernel
- **Firewall**: Security layer between kernel and agent, with predefined rules
- **Memory**: Dedicated data store containing conversation history and agent state

## Key Features

- **File Operations**: Read, write, update, and delete files with support for directory hierarchy traversal
- **System Monitoring**: Access to hardware and software information
- **Shell Integration**: Execute shell commands through a secure API
- **Directory Aliasing**: Simplified file access through human-friendly directory names
- **Secure Architecture**: Comprehensive firewall and guard protection
- **Agent Protocol Compatibility**: Full implementation of the Agent Protocol standard API

## Implementation Details

The platform is built on a service-oriented architecture with dependency injection:

- **Service Layer**: Handles file operations, directory services, and path resolution
- **Kernel Layer**: Processes agent requests and routes them to appropriate services
- **Security Layer**: Enforces access controls and verifies operation safety
- **API Layer**: RESTful API layer implementing the Agent Protocol standard

## Agent Protocol Integration

RoyaAI fully implements the [Agent Protocol](https://agentprotocol.ai) standard, providing a unified interface for agent-based systems. This allows RoyaAI to:

- Present a standardized API for agent interactions
- Enable interoperability with other Agent Protocol compatible systems
- Support agent tasks, steps, and artifacts management
- Provide webhooks for real-time notifications on agent events

The API endpoints adhere to the Agent Protocol specification, making RoyaAI compatible with any client designed to work with this standard.

## Getting Started

To work with the RoyaAI platform, you need to understand the fundamental interactions between agents and the kernel. The platform follows a request-response model where agents send structured requests to the kernel, which processes them and returns appropriate responses.

## Security Model

RoyaAI implements a rigorous security model:

- Firewall rules configurable only before startup through configuration files
- Guard system to prevent agents from accessing restricted resources
- Comprehensive health checks at startup to ensure system integrity

## About

This platform demonstrates how AI agents can safely and effectively interact with operating systems, providing a framework for developing more advanced AGI systems with real-world interaction capabilities.
