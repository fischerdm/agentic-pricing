# agentic-pricing

Shared foundation for agentic AI in insurance pricing.

This project is at an early stage. `agentic-pricing` is a meta-package that
installs the following components, which share the `agentic_pricing` namespace:

| PyPI package              | Import as                 | Purpose                                                       |
| ------------------------- | ------------------------- | ------------------------------------------------------------- |
| `agentic-pricing-core`    | `agentic_pricing.core`    | Line-of-business-agnostic building blocks for pricing agents. |
| `agentic-pricing-servers` | `agentic_pricing.servers` | Shared server infrastructure for exposing pricing agents.     |

It is used by the line-of-business projects built on top of it:

| Project                                          | Line of business                 |
| ------------------------------------------------ | -------------------------------- |
| [mammuthus](https://pypi.org/project/mammuthus/) | Non-life (P&C) insurance pricing |
| [olivetree](https://pypi.org/project/olivetree/) | Life insurance pricing           |

## Installation

```bash
pip install agentic-pricing
```
