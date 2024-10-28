# EnergyCo Project

This is a project repository for Team 2 members in FA24 BUSI 732 Quantitative Research course.

## 🐣 Project Setup Instructions

### 1. **Clone the repository**:

```bash
git clone https://github.com/busi732/Team-2-2024Fall.git
cd Team-2-2024Fall
```

💡 **VS Code Tip**: Use the integrated terminal to do this and set your Python interpreter to the new environment using `Ctrl+Shift+P` > `Python: Select Interpreter`.

### 2. **Create the environment** from the `environment.yml` file:

```bash
conda env create -f environment.yml
```

### 3. **Activate the environment**:

```bash
conda activate turbine
```

## 🌍 Environment Usage

### 🚀 Activate Your Environment:

Activate an environment by running:

```bash
conda activate turbine
```

You will know it's active when you see `(turbine)` in your terminal prompt.

💡 **VS Code Tip**: After activating the environment, set VS Code to use this environment:

1. Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on macOS).
2. Type `Python: Select Interpreter` and select your newly created `conda` environment.

### 🐍 Installing Packages with `conda` or `pip`

You can install packages using either `conda` or `pip`:

```bash
conda install <package_name>
```

or

```bash
pip install <package_name>
```

For example:

```bash
conda install numpy pandas
pip install requests
```

### Updating the Environment

Whenever `environment.yml` is updated, team members can update their environment by running:

```bash
conda env update --file environment.yml --prune
```

- The `--prune` flag removes the packages that are no longer required.

💡 Workflow for Team Members:

- When a team member **clones the repository** for the first time, they need to **create the conda environment** from the `environemtn.yml` file and **activate it** as described above.
- **Working on the Project**: After creating and activating the environment, team members can work on the project, install any necessary packages, and make their changes.
- **Installing or Updating Packages**: If a team member installs new packages that are important for the project, they should update the `environment.yml` file by running:

```bash
conda env export --no-builds > environment.yml
```

This updated file should then be **committed and pushed** to the repository.

- **Merging Updates**: When team members pull the latest changes from the repository, including an updated `environment.yml`, they need to update their local environment to match the new configuration:

```bash
conda env update --file environment.yml --prune
```

- The `--prune` flag ensures any packages removed from the environment are also removed locally, keeping everyone’s environment consistent.

💡 **Note**: The conda environment itself does **not** automatically merge. Updating the environment requires pulling the updated `environment.yml` and running `conda env update` manually to ensure all dependencies are consistent across team members.

## 🛠️ Helpful Tips

### Powershell Commands

**Clone repository**:

```bash
git clone https://github.com/busi732/Team-2-2024Fall.git
cd Team-2-2024Fall
```

**Create enviroment** from `environment.yml` file:

```bash
conda env create -f environment.yml
```

**Activate environment**:

```bash
conda activate turbine
```

**Update local environment**:

```bash
conda env update --file environment.yml --prune
```

**Export environment:**

```bash
conda env export --no-builds > environment.yml
```

- Run if packages have been installed or updated.

**Update packages**:

```bash
conda update --all
```

- Run periodically for up-to-date package compatibility.

**Install packages**:

```bash
conda install <package_name>
```

or

```bash
pip install <package_name>
```

### VSCode Shortcuts

| Action                        | Shortcut           |
| -                             | -                  |
| Terminal                      | ``Ctrl + ` ``      |
| Command Palette               | `Ctrk + Shift + P` |
| Markdown Preview Side-by-Side | `Ctrl + K V`       |

### Emoji Shortcuts

| OS      | Shortcut             |
| -       | -                    |
| Windows | `Windows key + .`    |
| Mac     | `Ctrl + Cmd + Space` |