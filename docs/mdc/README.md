# Model-Driven Configuration (MDC) Files

This directory contains Model-Driven Configuration files that guide the development of the NHL API Python client project.

## MDC Files Overview

### 📋 [project.mdc](./project.mdc)
- **Purpose**: Overall project overview and goals
- **Contents**: Project structure, technology stack, success criteria
- **Use**: Reference for project scope and objectives

### 🔌 [api.mdc](./api.mdc)
- **Purpose**: NHL API specification and data models
- **Contents**: Endpoints, data types, error handling, rate limiting
- **Use**: Guide for API implementation and data structures

### 🏗️ [architecture.mdc](./architecture.mdc)
- **Purpose**: Technical architecture and design patterns
- **Contents**: System components, design patterns, configuration
- **Use**: Reference for code organization and patterns

### 👨‍💻 [development.mdc](./development.mdc)
- **Purpose**: Development workflow and standards
- **Contents**: Coding standards, testing strategy, git workflow
- **Use**: Guide for development practices and quality assurance

### 🗺️ [roadmap.mdc](./roadmap.mdc)
- **Purpose**: Development phases and timeline
- **Contents**: Milestones, deliverables, success metrics
- **Use**: Project planning and progress tracking

## Technology Stack

- **Language**: Python 3.11+
- **Package Manager**: uv
- **Testing**: pytest
- **Linting**: ruff
- **Formatting**: black
- **Type Checking**: mypy
- **Documentation**: Sphinx

## Usage

These MDC files serve as the "source of truth" for the project. They should be:

1. **Referenced** during development decisions
2. **Updated** as the project evolves
3. **Followed** for consistency and quality
4. **Shared** with team members and contributors

## MDC Configuration

These MDC files are configured to be automatically applied in Cursor using YAML frontmatter at the top of each file:

```yaml
---
description: "Brief description of the MDC file's purpose"
globs: ["file patterns this MDC applies to"]
alwaysApply: true
---
```

### Configuration Options:

- **`description`**: Human-readable description of the MDC file's purpose
- **`globs`**: Array of file patterns where this MDC should be applied
  - `**/*.py` - All Python files
  - `src/nhl_api/**/*.py` - Specific package files
  - `tests/**/*.py` - Test files
  - `**/*.md` - Documentation files
  - `pyproject.toml` - Project configuration
- **`alwaysApply`**: When `true`, the MDC is automatically applied to matching files

### How It Works:

1. **Automatic Application**: When you open or create files matching the glob patterns, Cursor will automatically apply the relevant MDC guidance
2. **Context-Aware**: Different MDC files apply to different file types and locations
3. **Consistent Standards**: Ensures all code follows the defined architecture and standards
4. **Real-time Guidance**: Provides immediate feedback and suggestions as you code

### Current Configuration:

- **`project.mdc`**: Applies to all project files (Python, Markdown, config files)
- **`api.mdc`**: Applies to API-related Python files
- **`architecture.mdc`**: Applies to core package and test files
- **`development.mdc`**: Applies to all Python files and configuration files
- **`roadmap.mdc`**: Applies to project documentation and configuration files

## Contributing

When updating these files:
1. Ensure changes align with project goals
2. Update related files for consistency
3. Document significant changes
4. Review with team members if applicable
