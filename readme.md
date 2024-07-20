# miniRT

`miniRT` is a ray tracing project that generates images from scene descriptions. It uses geometric objects and lighting to create realistic images.

## Features
- **Objects**: Plane, Sphere, Cylinder
- **Transformations**: Translation, Rotation
- **Lighting**: Ambient, Diffuse, Hard Shadows
- **Window Management**: Resizable and closable with ESC or the red cross

## Usage
    To run the program, provide a `.rt` scene description file:
    ```sh
    ./miniRT scene.rt
    ```

## Installation
    - Clone the repository: 
        https://github.com/NuIled/miniRT.git

    - Navigate to the project directory:
        cd miniRT

    - Build the project:
        make

## Makefile Rules
    - all: Build the project
    - clean: Remove object files
    - fclean: Remove object files and binary
    - re: Rebuild the project
    - bonus: Build bonus files

## External Functions Used

    - open, close, read, write, printf, malloc, free, perror, strerror, exit
    - Math library (-lm)
    - MiniLibX

## Example Scene
    A 0.2 255,255,255
    C -50,0,20 0,0,0 70
    L -40,0,30 0.7 255,255,255
    pl 0,0,0 0,1.0,0 255,0,225
    sp 0,0,20 20 255,0,0
    cy 50.0,0.0,20.6 0,0,1.0 14.2 21.42 10,0,255
