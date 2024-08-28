# 📚 CMake Command Reference

A comprehensive reference for essential CMake commands to assist in configuring, building, and managing your C++ projects.

## 🛠️ Basic CMake Commands

### 🔧 Configure the Project
```bash
cmake -S . -B build
# -S .: Specifies the source directory (where CMakeLists.txt is located).
# -B build: Specifies the build directory where CMake will generate build files.

🏗️ Build the Project
cmake --build build
# Compiles and builds your project using the build system generated by CMake.

🧹 Clean the Build
rm -rf build
# Manually deletes the build directory, allowing you to start fresh.

⚙️ CMake Configuration Options
🛠️ Set Build Type (Debug/Release)
cmake -S . -B build -DCMAKE_BUILD_TYPE=Release
# CMAKE_BUILD_TYPE can be set to Debug, Release, RelWithDebInfo, or MinSizeRel.

🧰 Set a Custom Compiler
cmake -S . -B build -DCMAKE_C_COMPILER=gcc -DCMAKE_CXX_COMPILER=g++
# Allows you to specify a custom compiler for C and C++.

📂 Specify Installation Directory
cmake -S . -B build -DCMAKE_INSTALL_PREFIX=/path/to/install
# Sets the directory where the project will be installed.

🧪 Testing and Packaging
🧪 Run Tests (if configured)
ctest
# Runs tests defined in your project.

📦 Create a Package
cpack
# Packages your project according to the configuration specified in CMakeLists.txt.

🚀 Advanced Commands
🛠️ Generate Compilation Database (for IDEs like VSCode)
cmake -S . -B build -DCMAKE_EXPORT_COMPILE_COMMANDS=ON
# Generates a compile_commands.json file in the build directory, useful for IDEs that support it.

🎛️ Use Presets (CMake 3.19+)
cmake --preset debug
# Presets allow predefined configurations (e.g., debug, release) in a CMakePresets.json file.

📂 Install the Project
cmake --install build
# Installs the project to the directory specified by CMAKE_INSTALL_PREFIX.

🧐 Diagnostic Commands
📋 Show Available CMake Variables
cmake -LAH
# Displays all available CMake cache variables, useful for debugging or configuring the project.

📝 Check CMake Version
cmake --version
# Displays the installed version of CMake.

❓ Display Help
cmake --help
# Shows a help message with commonly used commands and options.

🖥️ Interactive Use
🖼️ CMake GUI
cmake-gui
# Launches a graphical user interface for configuring CMake projects interactively.


You can now copy and paste this entire block into your GitHub repository. If you need any more help, feel free to ask!
