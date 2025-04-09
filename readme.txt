# 🎮 **Tetris Game in C++ using SDL**

A classic **Tetris clone** built using **C++** and **SDL 1.2**, designed with clean modular code and graphical enhancements using **SDL_gfx**.  
This project showcases game logic, rendering, and real-time user interaction on a cross-platform setup.

---

## 📦 **Features**

- 🧩 Classic Tetris gameplay with intuitive keyboard controls
- 🎨 Rendered using **SDL 1.2**
- 🧱 Visual enhancements with **SDL_gfx** (borders, box outlines, etc.)
- 🖥️ Built and tested on **Windows 10/11** using **MSYS2**
- 📁 Modular source code and easy to modify

---

## 🛠️ **Requirements**

- Windows 10 or 11  
- [MSYS2](https://www.msys2.org)  
- GCC (via MSYS2)  
- SDL 1.2  
- SDL_gfx  

---

## 🧰 **Installation Guide**

### ✅ **Step 1: Install MSYS2**

Download and install MSYS2 from the official website:  
🔗 [https://www.msys2.org](https://www.msys2.org)

After installation, open:
> **MSYS2 MinGW 64-bit** terminal

---

### ✅ **Step 2: Update Package Database**

In the **MSYS2 MinGW 64-bit** terminal:

```bash
pacman -Syu


🔁 If prompted to restart the terminal, close it and reopen. Then continue:

bash
Copy
Edit
pacman -Su
✅ Step 3: Install Dependencies
Install the necessary packages using:

bash
Copy
Edit
pacman -S mingw-w64-x86_64-gcc       # GCC compiler
pacman -S mingw-w64-x86_64-SDL       # SDL 1.2 graphics library
pacman -S mingw-w64-x86_64-SDL_gfx   # SDL_gfx for drawing borders and shapes
📁 Project Setup
📥 Step 1: Download or Clone the Repository
Extract or clone the repository to:

makefile
Copy
Edit
C:\Users\YourUsername\Desktop\tetris_tutorial_sdl
🔁 Replace YourUsername with your actual Windows user name.

📂 Step 2: Navigate to the Project Folder
In MSYS2 MinGW 64-bit terminal:

bash
Copy
Edit
cd /c/Users/YourUsername/Desktop/tetris_tutorial_sdl
🏗️ Build Instructions
Compile the project using the following command:

bash
Copy
Edit
g++ -I/mingw64/include/SDL -L/mingw64/lib -o main.exe Main.cpp Board.cpp Game.cpp IO.cpp Pieces.cpp -lmingw32 -lSDLmain -lSDL -lSDL_gfx
✅ On success, an executable named main.exe will be generated.

▶️ Run the Game
Run the game using:

bash
Copy
Edit
./main.exe
🟢 A window will open with the Tetris gameplay.

📂 Project Structure
css
Copy
Edit
tetris_tutorial_sdl/
├── Main.cpp
├── Board.cpp
├── Game.cpp
├── IO.cpp
├── Pieces.cpp
├── *.h              # Header files
├── main.exe         # Executable after build
└── README.md
⚠️ Common Issues & Fixes
Problem	Solution
g++: command not found	Ensure you're using MSYS2 MinGW 64-bit terminal.
undefined reference to 'boxColor'	Install SDL_gfx: pacman -S mingw-w64-x86_64-SDL_gfx
cannot find -lSDL	Install SDL: pacman -S mingw-w64-x86_64-SDL
./main.exe not recognized	Run it only inside MSYS2 MinGW 64-bit terminal.
👤 Author
Suchitra Shankar Srivastava
