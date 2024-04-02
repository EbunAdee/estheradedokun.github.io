# The Maze Project 👨‍🎓 

![8970c3ee63d8149b93e30229276c3f7580ac9447]
This project is a first person `3D` maze game. Similar to Wolfenstein or Doom, minus enemies and weapons, although they may be added later. It was made using `SDL2` and `C`. It runs on Mac OS X and Linux/Ubuntu. The game uses the technique raycasting to create the apparent `3D` nature of the maze. The Maze is a 3D Maze game that uses ray casting to render a 2D map into a 3D navigable world! 

The Maze was written  in C using `SDL2` library. Deveploment was performed using Ubuntu 14.04 LTS - gcc (Ubuntu 4.8.4-2ubuntu1~14.04) 4.8.4

### About SDL2 💻
Simple DirectMedia Layer is a cross-platform development library designed to provide low level access to audio, keyboard, mouse, joystick, and graphics hardware via OpenGL and Direct3D. It is used by video playback software, emulators, and popular games including Valve's award winning catalog and many Humble Bundle games.

## Requirements to Play
- Mac OS X or Linux/Ubuntu
- SDL2

If you don't have SDL2 installed download the installation script <a href="https://s3.amazonaws.com/intranet-projects-files/holbertonschool-low_level_programming/graphics_programming/install_SDL2.sh">here</a>. Then find the script and run it in your terminal:
```groovy
$ ls
install_SDL2.sh
$ chmod 755 install_SDL2.sh
$ sudo ./install_SDL2.sh
```

## Start the Game
First step is to clone the repo:
```groovy
git clone https://github.com/EbunAdee/the-maze_project.git
```

Compile all .c files in the maze directory:
```groovy
root@26acb882cd08:/estheradedokun.github.io# gcc -g -Wall -Werror -Wextra -pedantic -I/usr/local/include/SDL2 ./src/*.c -o maze -L/usr/lib/x86_64-linux-gnu -lSDL2 -lm
```
Alternatively, just use the make command:
```sh
make
```

Run the maze with the map you'd like to play:
```groovy
./maze maps/level_1
```
Or you can run with multiple maps at once:
```groovy
./maze maps/level_1 maps/level_2
```

Some basic maps are provided in this repo in the maps/ directory, but you can make your own maps to play as well.

After running `./maze maps/level_1` you should see a screen like this:

![Screenshot from 2023-11-21 10-23-10]
If you're using the provided maps it'll just be a red screen, but that's not all. If you rotate with the arrow keys to the right you'll see the rest of the maze:

![Screenshot from 2023-11-21 10-27-31]
## Play the Game
The goal of the game is to find the end of the maze. To move through the maze use the arrow keys. The left and right arrow keys will rotate the player. The up and down arrow keys will move the player forward or backward.

Currently the player's starting position and the end goal position of the maze can be decided when creating the map file. If no positions are stated in the file then the player starts in the top left corner and the goal will be in the last floor space in the file.

When you have found the end of the maze you will either move, rather abruptly, to the next maze or the game will exit and you will be greeted with a win message in your console.

## Creating a Maze
The files in the `maps/` directory provide examples of the file format for a maze to work with this game. The different characters in the file represent different colored walls, the floor, the player position, or the position of the end goal.

**Map File Characters' in Game Meanings**
- **0**: Floor/walkable space
- **1**: Red Wall
- **2**: Green Wall
- **3**: Blue Wall
- **4**: Yellow Wall
- **w**: End goal
- **p**: Player start position
- All other characters will be defaulted to white walls

## Flowchart
![The Maze Flow Chart](https://i.imgur.com/t0MxNni.png)

## Reference
- [lazyfoo](http://lazyfoo.net/tutorials/SDL/index.php#Event%20Driven%20Programming)
- [geeksforgeeks](https://www.geeksforgeeks.org/structure-vs-class-in-cpp/)
- [permadi.com](https://permadi.com/1996/05/ray-casting-tutorial-1/)
- [lodev.org](https://lodev.org/cgtutor/raycasting.html)
- [cplusplus.com](https://cplusplus.com/forum/beginner/214311/)
- [pikuma.com](https://pikuma.com/courses/raycasting-engine-tutorial-algorithm-javascript)
- [3DSage/OpenGL-Raycaster](https://www.youtube.com/watch?v=gYRrGTC7GtA)


<details><summary align="center"> </samp></summary><p align ="center"> Click on The PICTURE☝️</p></details>

<p align="center">
<b align="center">📍This project is still a work in progress more detail on the project will be available in the future🍿📺🍿</b>

## Author :black_nib:
1. _[ESTHER ADEDOKUN] | [Github](https://github.com/EbunAdee) | [Linkedin](https://www.linkedin.com/in/adedokun-esther-2a91a5122) | [Twitter](https://twitter.com/EbunAde)._

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

# Acknowledgements 🙏
All work contained in this project was completed as part of the curriculum for _Alx-Africa_. _Alx-Africa_ is a remote-based full-stack software engineering program that prepares students for careers in the tech industry using project-based peer learning. For more information, visit this [link](https://www.alxafrica.com/).
* **ALX staff**: For the help, advice, and resources throughout the project and curriculum.
* **Cohort 17 and all ALX students**: For friendship, support, and insights over the last year.
* **YOU**: For reading this documentation and testing out The Game. I hope you enjoyed the ride!

## Support🎉
If you like how I present and document my work do me a favor of giving a Star ✨ to my [Repos](https://https://github.com/EbunAdee/estheradedokun.github.io) |&&| a [Follow](https://github.com/EbunAdee) 👥

<p align="center">
<h2 align="center"><img align="center" src="https://github.com/elyse502/AirBnB_clone/assets/125453474/ab3c1e01-2b98-47ae-96b7-37c07c85a2f1" alt="footer" width="150"  height="150"/></h2>






