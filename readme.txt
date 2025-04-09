# 🎮 Tetris Game in C++ using SDL

A classic **Tetris clone** built using **C++** and **SDL 1.2** graphics.  
The project also utilizes **SDL_gfx** for drawing additional elements like borders and boxes.

---

## 📦 Features

- Tetris gameplay with simple, intuitive controls
- Uses SDL for rendering and event handling
- SDL_gfx used for drawing shapes (like boxes around pieces)
- Cross-platform support via SDL (built for Windows via MSYS2)

---

## 🛠 Requirements

- Windows 10/11
- [MSYS2](https://www.msys2.org)
- g++ (C++ Compiler)
- SDL 1.2
- SDL_gfx

---

## 🧰 Installation Guide

### ✅ Step 1: Install MSYS2

Download MSYS2 from the official website:  
🔗 https://www.msys2.org

Follow the installation instructions provided there.

After installation, open:
> **MSYS2 MinGW 64-bit** terminal from the Start Menu

---

### ✅ Step 2: Update the Package Database

In the **MSYS2 MinGW 64-bit terminal**, run:

```bash
pacman -Syu

🔁 If prompted to close the terminal after updating, do so.

Then reopen MSYS2 MinGW 64-bit and run:

bash
Copy
Edit
pacman -Su
✅ Step 3: Install Dependencies
Run the following commands in the terminal to install the required packages:

bash
Copy
Edit
pacman -S mingw-w64-x86_64-gcc       # C++ compiler
pacman -S mingw-w64-x86_64-SDL       # SDL 1.2 graphics library
pacman -S mingw-w64-x86_64-SDL_gfx   # SDL_gfx for drawing boxes and shapes
📁 Project Setup
Step 1: Download or Clone the Repository
If you downloaded the project as a ZIP file, extract it to a location like:

makefile
Copy
Edit
C:\Users\YourUsername\Desktop\tetris_tutorial_sdl
🔁 Replace YourUsername with your actual Windows username.

Step 2: Navigate to the Project Folder
Open the MSYS2 MinGW 64-bit terminal, then navigate to the project directory:

bash
Copy
Edit
cd /c/Users/YourUsername/Desktop/tetris_tutorial_sdl
🏗️ Building the Game
Once inside the project folder, compile the game using:

bash
Copy
Edit
g++ -I/mingw64/include/SDL -L/mingw64/lib -o main.exe Main.cpp Board.cpp Game.cpp IO.cpp Pieces.cpp -lmingw32 -lSDLmain -lSDL -lSDL_gfx
✅ If the compilation is successful, a file named main.exe will be created.

▶️ Running the Game
To run the game, simply execute:

bash
Copy
Edit
./main.exe
🟢 A new window should open, running the Tetris game!

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
├── Header Files (.h)
├── main.exe (after building)
└── README.md
🚧 Common Errors & Fixes
Problem	Fix
g++: command not found	Make sure you're using MSYS2 MinGW 64-bit, not the default MSYS terminal.
undefined reference to 'boxColor'	Install SDL_gfx: pacman -S mingw-w64-x86_64-SDL_gfx
cannot find -lSDL	Make sure SDL is installed: pacman -S mingw-w64-x86_64-SDL
./main.exe not recognized	Only works inside MSYS2 MinGW 64-bit terminal.
🧑‍💻 Author
Made by Suchitra Shankar Srivastava

