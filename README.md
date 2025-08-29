# NHL API Python Client

A comprehensive Python client for the NHL API, providing easy access to hockey data including teams, players, games, and statistics.

## 🏒 Overview

This project aims to create a clean, well-documented API wrapper for NHL data with type-safe interfaces, caching, and rate limiting for optimal performance. It provides a user-friendly interface for accessing hockey statistics, supporting both real-time game data and historical statistics.

## 🚀 Features

- **Type-Safe Interfaces**: Full type hints and Pydantic models for all NHL API endpoints
- **Comprehensive Coverage**: Access to teams, players, games, statistics, and more
- **Performance Optimized**: Built-in caching and rate limiting
- **Developer Friendly**: Clean API design with comprehensive documentation
- **Real-time Data**: Support for live game data and historical statistics

## 📋 Project Status

This project is currently in **development phase**. See the [roadmap](./docs/mdc/roadmap.mdc) for detailed development phases and timeline.

### Development Phases
1. **Phase 1**: Basic API client setup and core endpoints
2. **Phase 2**: Type definitions and error handling  
3. **Phase 3**: Caching and rate limiting
4. **Phase 4**: Advanced features and optimizations
5. **Phase 5**: Documentation and examples

## 🛠️ Technology Stack

- **Language**: Python 3.11+
- **Package Manager**: [uv](https://github.com/astral-sh/uv)
- **Testing**: [pytest](https://pytest.org/)
- **Linting**: [ruff](https://github.com/astral-sh/ruff)
- **Formatting**: [black](https://black.readthedocs.io/)
- **Type Checking**: [mypy](https://mypy-lang.org/)
- **Documentation**: [Sphinx](https://www.sphinx-doc.org/)

## 📁 Project Structure

```
nhl_apimdc/
├── src/
│   └── nhl_api/           # Main package
│       ├── __init__.py
│       ├── client.py      # Main API client
│       ├── endpoints/     # API endpoint modules
│       ├── models/        # Pydantic models
│       ├── utils/         # Utility functions
│       └── exceptions.py  # Custom exceptions
├── tests/                 # Test files
├── docs/                  # Documentation
│   └── mdc/              # Model-Driven Configuration files
├── examples/              # Usage examples
├── pyproject.toml         # Project configuration
├── .ruff.toml            # Ruff configuration
├── .mypy.ini             # MyPy configuration
└── README.md
```

## 📚 Documentation

This project uses **Model-Driven Configuration (MDC)** files to guide development and maintain consistency. All documentation is located in the `docs/mdc/` directory:

### Core Documentation Files

- **[Project Overview](./docs/mdc/project.mdc)** - Overall project goals and structure
- **[API Specification](./docs/mdc/api.mdc)** - NHL API endpoints and data models
- **[Architecture](./docs/mdc/architecture.mdc)** - Technical design and patterns
- **[Development Standards](./docs/mdc/development.mdc)** - Coding standards and workflow
- **[Roadmap](./docs/mdc/roadmap.mdc)** - Development phases and timeline

### Specialized Documentation

- **[Event Codes](./docs/mdc/event.mdc)** - NHL game event codes and descriptions
- **[Situation Codes](./docs/mdc/situation.mdc)** - Game situation codes and meanings
- **[Player Performance](./docs/mdc/player_performance.mdc)** - Player statistics and metrics
- **[Data Strategy](./docs/mdc/data_strategy.mdc)** - Data handling and caching strategies
- **[Type Codes](./docs/mdc/typecode.mdc)** - NHL API type code definitions

## 🏗️ Architecture

The project follows a clean architecture pattern with:

- **API Client Layer**: Handles HTTP requests and responses
- **Model Layer**: Pydantic models for type safety and validation
- **Endpoint Layer**: Organized API endpoint modules
- **Utility Layer**: Shared functionality and helpers
- **Exception Layer**: Custom error handling

## 🧪 Development

### Prerequisites

- Python 3.11 or higher
- [uv](https://github.com/astral-sh/uv) package manager

### Setup

```bash
# Clone the repository
git clone https://github.com/cooneycw/nhl_apimdc.git
cd nhl_apimdc

# Install dependencies
uv sync

# Run tests
uv run pytest

# Run linting
uv run ruff check .

# Run type checking
uv run mypy src/
```

### Development Workflow

1. **Code Standards**: Follow the guidelines in [development.mdc](./docs/mdc/development.mdc)
2. **Testing**: Maintain >90% test coverage
3. **Documentation**: Update MDC files as the project evolves
4. **Quality**: Use ruff for linting and black for formatting

## 🎯 Success Criteria

- [ ] All major NHL API endpoints are implemented
- [ ] Type definitions are complete and accurate
- [ ] Comprehensive test coverage (>90%)
- [ ] Well-documented API with examples
- [ ] Performance optimizations implemented
- [ ] Published to PyPI registry

## 🤝 Contributing

We welcome contributions! Please:

1. Follow the development standards in [development.mdc](./docs/mdc/development.mdc)
2. Update relevant MDC files for consistency
3. Add tests for new functionality
4. Document significant changes

## 📄 License

This project is open source. See the LICENSE file for details.

## 🔗 Links

- **Repository**: https://github.com/cooneycw/nhl_apimdc
- **NHL API**: https://statsapi.web.nhl.com/
- **Documentation**: See the `docs/mdc/` directory for detailed specifications

## 🙏 Credits

This project was inspired by and references the excellent [NHL API Reference](https://github.com/Zmalski/NHL-API-Reference) by [@Zmalski](https://github.com/Zmalski), which serves as the unofficial reference for NHL API endpoints. Their comprehensive documentation of the NHL APIs has been invaluable in understanding the available endpoints and data structures.

---

**Note**: This project is in active development. The API and documentation may change as the project evolves.
