# pixi-isaac

## Getting Started

1. Clone the repository. Issac Sim is available as pip packages, but Isaac Lab is not. Here, Isaac Lab is downloaded as a submodule and installed separately.
    ```
    git clone --recursive https://github.com/kywch/pixi-isaac.git
    ```

    Then, go to the repository directory.
    ```
    cd pixi-isaac
    ```

2. Using pixi, set up the virtual environment and install pytorch and Isaac Sim.

    Install pixi, if you haven't already. See [pixi documentation](https://pixi.sh/latest/#installation) for more details. The following command is for linux.
    ```
    curl -fsSL https://pixi.sh/install.sh | bash
    ```

    The following command sets up the virtual environment and installs the dependencies.
    ```
    pixi install
    ```

    The following command tests if gpu-enabled pytorch is installed.
    ```
    pixi run test_torch
    ```

    The following command tests if Isaac Sim is correctlyinstalled.
    ```
    pixi run isaacsim
    ```

3. Install and test Isaac Lab.

    The following command activates the virtual environment.
    ```
    pixi shell
    ```

    Install Isaac Lab.
    ```
    ./install_isaaclab.sh
    ```

    After the install, the following command should work within the activated virtual environment.
    ```
    python tutorials/00_sim/create_empty.py
    ```

    Or, without activating the virtual environment, you can run the following command.
    ```
    pixi run python tutorials/00_sim/create_empty.py
    ```
