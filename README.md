## Simple game project starting template in C99 with hot reloading

This is a template for me so I don't have to build the hot reloading every time I start a new project.

Posting this in case it's useful for someone else, I will try to keep updating this template as I use it to make it more complete.

The way it works is it separates the platform layer from the game layer, the game layer is compiled into a separated .so this is then dynamically loaded on the the platform
layer, every frame the platform layer checks if the file game so file has changed since last load and if it does it reloads it.

Currently only "platform" included is linux/raylib.

Just running ./scripts/build.sh will cause the platform layer to hot reload the game layer

https://github.com/user-attachments/assets/6f66a0f8-f30d-43fa-94cb-1c98efa7c09f

