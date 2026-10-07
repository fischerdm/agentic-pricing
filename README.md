# agentic-pricing

Shared foundation for agentic AI in insurance pricing.

This project is at an early stage. `agentic-pricing` is a meta-package that
installs the following components, which share the `agentic_pricing` namespace:

| PyPI package              | Import as                 | Purpose                                                              |
| ------------------------- | ------------------------- | -------------------------------------------------------------------- |
| `agentic-pricing-core`    | `agentic_pricing.core`    | Shared domain model, interfaces and configuration.                   |
| `agentic-pricing-tools`   | `agentic_pricing.tools`   | Building-block utilities used by agents.                             |
| `agentic-pricing-agents`  | `agentic_pricing.agents`  | Agentic components built on top of tools.                            |
| `agentic-pricing-mcp`     | `agentic_pricing.mcp`     | Shared MCP server infrastructure for exposing tools and agents.      |
| `agentic-pricing-servers` | `agentic_pricing.servers` | Shared infrastructure for exposing tools and agents as services.     |

It is used by the line-of-business projects built on top of it, which follow the
same layers (`-tools`, `-agents`, `-mcp`, `-servers`) and build on the matching
`agentic-pricing` package:

| Project                                          | Line of business                 |
| ------------------------------------------------ | -------------------------------- |
| [mammuthus](https://pypi.org/project/mammuthus/) | Non-life (P&C) insurance pricing |
| [olivetree](https://pypi.org/project/olivetree/) | Life insurance pricing           |

## Installation

```bash
pip install agentic-pricing
```
