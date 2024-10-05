#### Step 1: Download Docker Desktop
1. **Go to the Docker official website**: Visit [https://www.docker.com/products/docker-desktop](https://www.docker.com/products/docker-desktop).
2. **Download Docker Desktop for Windows**: Click the download button for Docker Desktop. Make sure to choose the correct version based on your system architecture (typically for 64-bit systems).

#### Step 2: Enable Virtualization
- Docker requires **virtualization** to run containers on Windows.
- To enable virtualization:
  1. **Open your BIOS/UEFI settings**: Restart your computer and press the designated key (such as F2, F10, Delete) to enter BIOS/UEFI.
  2. **Enable virtualization**: Look for a setting like "Intel VT-x," "Intel Virtualization Technology," or "AMD-V" and enable it.
  3. **Save and exit**: Save changes and restart your computer.

#### Step 3: Install Docker Desktop
1. **Run the installer**: Once the Docker Desktop executable has been downloaded, run the installer.
2. **Choose configuration options**: During installation, you can choose to enable:
   - **Use WSL 2** (Windows Subsystem for Linux 2): This is recommended for better performance and compatibility with Linux containers.
   - **Add Docker to your PATH**: This allows you to use Docker from any command prompt window.
3. **Click Install**: Follow the prompts and wait for the installation to complete.

#### Step 4: Start Docker Desktop
- After the installation is complete, **launch Docker Desktop** from the Start menu or desktop shortcut.
- **Log in or create an account**: You will be prompted to log in to Docker Hub (or create a free account if you don’t have one).
- Docker will start automatically in the background, and you should see the Docker icon in your system tray.

#### Step 5: Verify Docker Installation
1. **Open PowerShell** or **Command Prompt**.
2. Run the command to verify installation:
   ```bash
   docker --version
   ```
   This should display the Docker version if the installation was successful.

#### Step 6: Configure WSL 2 (Optional)
- If you enabled **WSL 2** during installation, you may need to ensure that WSL 2 is properly set up on your machine.
  1. Open PowerShell and run:
     ```bash
     wsl --list --verbose
     ```
  2. If WSL 2 is not the default version, set it by running:
     ```bash
     wsl --set-default-version 2
     ```
  3. Ensure that your distributions are running under WSL 2.

#### Step 7: Test Docker Installation
1. To confirm Docker is working, run the **hello-world** container:
   ```bash
   docker run hello-world
   ```
   This will download and run a simple Docker container that outputs a confirmation message.