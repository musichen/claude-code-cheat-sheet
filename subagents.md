# Claude Code Subagents

> **A comprehensive guide to specialized agents in Claude Code - maximize your productivity with targeted AI assistance**

Claude Code features powerful specialized subagents designed to handle specific types of development tasks. Each subagent is optimized for particular workflows and comes with specialized tools and knowledge domains.

## 📋 Table of Contents

- [Overview](#overview)
- [Available Subagents](#available-subagents)
- [Quick Reference](#quick-reference)
- [Best Practices](#best-practices)
- [Integration Workflows](#integration-workflows)

## Overview

Subagents in Claude Code provide specialized expertise for different aspects of software development. Instead of using a general-purpose agent for all tasks, you can leverage these focused agents to get better results for specific use cases.

### Key Benefits

- **Specialized Knowledge**: Each agent has domain-specific expertise
- **Optimized Tools**: Agents have access to tools most relevant to their specialty
- **Better Context**: Focused agents maintain context relevant to their domain
- **Faster Results**: Specialized agents can work more efficiently in their area

## Available Subagents

### Development Specialists

#### [Frontend Developer](subagents/frontend-developer.md)
Specialized for building, modifying, and debugging frontend components, UI elements, styling, and user interface logic.

#### [Backend Developer](subagents/backend-developer.md)
Expert in server-side development, APIs, databases, and system architecture.

#### [API Developer](subagents/api-developer.md)
Focused on API design, implementation, documentation, and integration.

#### [Mobile Developer](subagents/mobile-developer.md)
Specialized in mobile application development for iOS and Android platforms.

### Language Specialists

#### [Python Developer](subagents/python-developer.md)
Expert in Python development, frameworks, and ecosystem tools.

#### [JavaScript Developer](subagents/javascript-developer.md)
Specialized in JavaScript development, Node.js, and browser-based applications.

#### [TypeScript Developer](subagents/typescript-developer.md)
Expert in TypeScript development, type systems, and modern JavaScript patterns.

#### [PHP Developer](subagents/php-developer.md)
Specialized in PHP development, frameworks, and web application development.

#### [WordPress Developer](subagents/wordpress-developer.md)
Expert in WordPress development, themes, plugins, and customization.

#### [iOS Developer](subagents/ios-developer.md)
Specialized in iOS application development using Swift and Objective-C.

### Database & Architecture

#### [Database Designer](subagents/database-designer.md)
Expert in database design, optimization, and data modeling.

### Code Quality & Maintenance

#### [Code Reviewer](subagents/code-reviewer.md)
Specialized in code review, quality assessment, and best practices enforcement.

#### [Code Debugger](subagents/code-debugger.md)
Expert in debugging, troubleshooting, and problem resolution.

#### [Code Documenter](subagents/code-documenter.md)
Specialized in creating comprehensive documentation for codebases.

#### [Code Refactor](subagents/code-refactor.md)
Expert in code refactoring, optimization, and restructuring.

#### [Code Security Auditor](subagents/code-security-auditor.md)
Specialized in security analysis, vulnerability assessment, and secure coding practices.

#### [Code Standards Enforcer](subagents/code-standards-enforcer.md)
Expert in coding standards, style guides, and code consistency enforcement.

## Quick Reference

### When to Use Each Subagent

| Task Type | Recommended Subagent | Example Use Case |
|-----------|---------------------|------------------|
| Building UI components | Frontend UI Expert | "Create a responsive navigation bar" |
| Code quality review | Production Validator | "Review this code for production readiness" |
| Writing documentation | Code Documentor | "Document this authentication module" |
| Complex research | General Purpose | "Find all API endpoints in this codebase" |
| Multi-step automation | General Purpose | "Set up CI/CD pipeline with testing" |

### Subagent Invocation Patterns

```bash
# Using Task tool to invoke subagents
/task description="Build user profile component" subagent_type="frontend-ui-expert"
/task description="Review code quality" subagent_type="production-validator"
/task description="Create API docs" subagent_type="code-documentor"
/task description="Research database schema" subagent_type="general-purpose"
```

## Best Practices

### Choosing the Right Subagent

1. **Match Task to Expertise**: Choose the subagent whose specialty aligns with your task
2. **Consider Tool Requirements**: Some subagents have limited tool access by design
3. **Think About Context**: Specialized agents maintain better focused context
4. **Use General Purpose for Complex Tasks**: When tasks span multiple domains, use the general-purpose agent

### Effective Subagent Usage

1. **Be Specific**: Provide clear, detailed task descriptions
2. **Set Clear Expectations**: Specify what you want the subagent to deliver
3. **Provide Context**: Include relevant background information
4. **Chain Subagents**: Use multiple subagents in sequence for complex workflows

### Common Patterns

```bash
# Frontend Development Workflow
1. Frontend UI Expert: Build component
2. Production Validator: Review for production
3. Code Documentor: Create component documentation

# Code Review Workflow  
1. Production Validator: Initial quality check
2. General Purpose: Complex analysis if needed
3. Code Documentor: Update documentation

# Research and Implementation
1. General Purpose: Research and planning
2. Specialized Agent: Implementation
3. Production Validator: Final review
```

## Integration Workflows

### Multi-Agent Workflows

Claude Code allows you to chain subagents together for complex workflows:

1. **Sequential Processing**: Use agents one after another
2. **Parallel Processing**: Run multiple agents concurrently
3. **Conditional Logic**: Choose agents based on task requirements

### Example Workflows

#### Complete Feature Development
```
1. General Purpose: Research requirements and plan architecture
2. Frontend UI Expert: Build user interface components  
3. Production Validator: Review code quality and security
4. Code Documentor: Create comprehensive documentation
```

#### Code Quality Pipeline
```
1. Production Validator: Automated quality checks
2. General Purpose: Complex issue analysis (if needed)
3. Frontend UI Expert: UI-specific fixes (if applicable)
4. Code Documentor: Update documentation
```

## Getting Started

1. **Identify Your Task Type**: Determine which subagent is most appropriate
2. **Use the Task Tool**: Invoke the subagent using Claude Code's Task tool
3. **Provide Clear Instructions**: Be specific about what you want accomplished
4. **Review Results**: Each subagent will provide a focused response
5. **Chain as Needed**: Use multiple subagents for complex workflows

## Advanced Usage

### Custom Subagent Patterns

You can create sophisticated workflows by combining subagents with Claude Code's other features:

- **Session Management**: Maintain context across subagent invocations
- **Tool Permissions**: Configure specific tool access for security
- **Output Formatting**: Use structured output for automation
- **Error Handling**: Implement fallback patterns between subagents

### Performance Optimization

- Use specialized subagents to reduce context switching
- Leverage parallel subagent execution when possible
- Cache common subagent results for repeated tasks
- Monitor subagent performance with Claude Code's cost tracking

---

For detailed information about each subagent, see the individual documentation files in the `subagents/` directory.