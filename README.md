# Blade Gunner 2049

This is a 2D top-down shooter game developed using the **Raylib** game development library. The game features a player who fights against waves of enemies, using guns, speed boosts, and dashes to survive as long as possible.

## Table of Contents
- [General Information](#general-information)
- [Technologies Used](#technologies-used)
- [Setup](#setup)
- [How to Play](#how-to-play)
- [Features](#features)
- [Game Assets](#game-assets)
- [License](#license)
  
## General Information
**Blade Gunner 2049** is a fast-paced shooting game where the player must defeat incoming enemies while managing limited resources such as health, dash abilities, and speed boosts. The player earns XP and levels up as they eliminate enemies, which increases the difficulty of the game.

Developed by:
- Zeyad Ayman Mahmoud, ID: 211009779

## Technologies Used
- **Raylib** - A simple and easy-to-use library to enjoy videogames programming.
- **C Language** - The core language used for the game's development.
- **Raymath** - For handling vector operations like player and bullet positioning.
- **Raylib Audio** - For loading and managing sound effects and music in the game.

## Setup

1. **Install Raylib**:
    - Follow the instructions to install [Raylib](https://www.raylib.com/) on your system.

2. **Clone the Repository**:
    ```bash
    git clone https://github.com/username/blade-gunner-2049.git
    cd blade-gunner-2049
    ```

3. **Build and Run the Game**:
    - Compile the game using your preferred compiler with Raylib linked:
    ```bash
    gcc -o blade_gunner main.c -lraylib -lGL -lm -lpthread -ldl -lrt -lX11
    ./blade_gunner
    ```

4. **Required Assets**:
    - Place all assets (images, sounds, and music) in the `resources/` directory.
    - The required assets include background images, player and enemy sprites, bullets, icons, and sound effects (detailed below).

## How to Play

- **Movement**: 
    - Use **WASD** keys to move the player.
  
- **Shooting**: 
    - Aim with the mouse and click the **left mouse button** to shoot.

- **Speed Boost**: 
    - Press **Spacebar** to activate a temporary speed boost.

- **Dash**: 
    - Press **C** to dash in the current movement direction. Dashing allows you to avoid enemy attacks.

- **Pause**:
    - The game can be paused by pressing **X** (unpauses and adjusts difficulty).

- **XP and Levels**:
    - Kill enemies to earn XP and level up. The XP requirement increases after each level.

- **Enemies**:
    - Two types of enemies spawn at random locations and chase the player. 

## Features
- **Enemies**:
    - Random spawning with varying types.
    - Basic enemy AI that follows the player.
  
- **Shooting**:
    - Player can shoot bullets, and these bullets have limited lifetime and speed.

- **Timers**:
    - Implemented timers for bullet lifespan, speed boost, and dash cooldowns.

- **Camera**:
    - Camera follows the player's movement, keeping the player in the center of the screen.

- **Collision Detection**:
    - Bullets and enemies have collision detection, causing health reduction or destruction.

- **Power-ups**:
    - Speed boost increases player movement speed for a limited time.
    - Dashes provide quick evasive movements.

## Game Assets

All assets must be placed in the `resources/` directory:

1. **Background Image**: `resources/bgfinal.png`
2. **Player Texture**: `resources/mc_walk_with_gun.png`
3. **Enemy Textures**: 
   - `resources/enemy_2.png`
   - `resources/enemy_1.png`
4. **Bullet Texture**: `resources/bullet3s.png`
5. **Icons**: 
   - Speed boost: `resources/speed_boost_icon.png`
   - Speed boost cooldown: `resources/speed_boost_cooldown.png`
   - Dash: `resources/dash_icon.png`
   - Dash cooldown: `resources/dash_icon_cooldown.png`
6. **Audio Files**:
   - Background music: `resources/musicc.mp3`
   - Shooting sound: `resources/shoot.wav`
   - Enemy hurt sound: `resources/enemyhurt.ogg`
   - Player hurt sound: `resources/playerhurt.mp3`
   - Level up sound: `resources/lvlup.wav`
7. **High Score File**: `resources/Scores.txt` (stores player's high score)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Have fun playing **Blade Gunner 2049**!
