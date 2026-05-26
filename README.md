# sdk

> Python client SDK for interacting with the core inference API - part of the [TensorRelay](https://github.com/TensorRelay) open-source ecosystem.

## Overview

Designed for ML engineering teams that need more than a hosted API. This project handles the hard parts of running AI in production - inference routing, scaling, failover, and observability - so you can focus on model quality instead of infrastructure.

The `sdk` package provides the Python interface for integrating with TensorRelay's infrastructure, designed for ease of use in both scripts and production services.

## Features

- Distributed inference serving with sub-50ms p99 latency
- Horizontal scaling across GPU and CPU clusters
- Built-in model versioning and A/B traffic splitting
- OpenTelemetry-native observability and tracing
- Pluggable storage backends (S3, GCS, local)

## Requirements

- Python 3.11 or later
- pip or [uv](https://github.com/astral-sh/uv) (recommended)

## Installation

```bash
pip install sdk
```

Or from source:

```bash
git clone https://github.com/TensorRelay/sdk
cd sdk
pip install -e .
```

## Usage

```python
from sdk import Client

client = Client()
# See documentation for full API reference
```

## Development

```bash
# Install dev dependencies
pip install -e ".[dev]"

# Run tests
pytest

# Lint
ruff check .
```

## Contributing

Contributions are welcome and appreciated! Here's how to get started:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/my-feature`)
3. Make your changes with tests
4. Commit using conventional commits (`git commit -m 'feat: add my feature'`)
5. Push to your fork and open a Pull Request

Please read our contribution guidelines before submitting. All contributors are expected to follow our code of conduct.

## Contact & Support

Have a question, found a bug, or want to collaborate?

- **Email:** [rk822827@gmail.com](mailto:rk822827@gmail.com)
- **GitHub Issues:** [github.com/TensorRelay/issues](https://github.com/TensorRelay)
- **Discussions:** [github.com/TensorRelay/discussions](https://github.com/TensorRelay)

We aim to respond to all inquiries within 48 hours.

## License

Released under the [MIT License](LICENSE). See `LICENSE` for full details.
