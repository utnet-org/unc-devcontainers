# Devcontainer for Utility Smart Contract

This repository hosts the official Devcontainer image for Utility contract development, featuring preinstalled essential tools. You can access the image on the [GitHub Container Registry](https://ghcr.io/utnet-org/unc-devcontainer).

## Usage

To incorporate this Devcontainer into your own repositories, follow these steps:

1. Fork the [Utility Rust Stack template repo](https://github.com/utnet-org/unc-new-project-template).
2. Open the forked repository in Codespaces.

For integrating this Devcontainer into your repositories, create the following configuration in `.devcontainer/devcontainer.json`:

```json
{
  "name": "Utility Devcontainer Rust",
  "image": "ghcr.io/utnet-org/utility-devcontainers-rs:latest",
  // Uncomment and modify the following lines if necessary
  // "forwardPorts": [8000],
  "customizations": {
    "codespaces": {
      // Uncomment and modify the following lines if necessary
      // "openFiles": ["README.md", "src/lib.rs", "tests/test_basics.rs"]
    }
  }
}
```

## Features

The `unc-cli` features are available separately and can be used in other Devcontainers. Include the following configurations in your `.devcontainer/devcontainer.json`:

For `unc-cli`:

```json
"features": {
  "ghcr.io/utnet-org/utility-devcontainers-rs/features/unc-cli:latest": {}
}
```

## Contributing

Feel free to contribute to this Devcontainer repository. Any issues or improvements can be raised through the GitHub repository's issue tracker.
