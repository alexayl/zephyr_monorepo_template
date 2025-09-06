# Zephyr Monorepo Template

A template repository for managing a monorepo containing a Zephyr project.


## Setup

0. Install prerequisites

    - [Python3](https://www.geeksforgeeks.org/python/download-and-install-python-3-latest-version/)

    - Complete **only** the following sections of the [Getting Started Guide](https://docs.zephyrproject.org/latest/develop/getting_started/index.html#getting-started-guide).
        - [Install Dependencies](https://docs.zephyrproject.org/latest/develop/getting_started/index.html#install-dependencies)
        - Skip *Get Zephyr and install Python dependencies*
        - [Install the Zephyr SDK](https://docs.zephyrproject.org/latest/develop/getting_started/index.html#install-the-zephyr-sdk)

    - [Just command runner](https://github.com/casey/just?tab=readme-ov-file#installation) - This is used like a makefile as a hotkey for all of our project-specific commands

1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/zephyr_monorepo_template.git
    cd zephyr_monorepo_template
    ```

2. Create and activate a Python virtual environment:
    ```bash
    python -m venv .venv
    source .venv/bin/activate  # On Linux/macOS
    ```

3. Install west
    ```bash
    pip install west
    ```

4. Update the workspace
    ```bash
    cd firmware
    west update
    ```

5. Install other python packages
    ```bash
    west packages pip --install
    ```
6. Try to build and run
    ```bash
    just run-sim
    ```