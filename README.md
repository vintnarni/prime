# prime.sh

> [!WARNING]
> I no longer have an computer that has NVIDIA graphics card, so i decided to archive the repository for historical reasons, thus no support will be provided.

A really simple script i made in ~30 seconds, (un)licensed under [Unlicense](https://unlicense.org/), to run any application using NVIDIA discrete GPU.

It requires even less typing time and dead simple to remember, no questions asked.

Useful if you have Optimus-enabled device.

The reason why i made this is because i'm using it in case either `nvidia-prime` or similar name wasn't available in my distro or was too hard to install.

## How do i use it?

It's as simple as cloning this repo and typing `prime [insert_program_name]` there in your terminal (replace `[insert_program_name]` with your preferred program).

## How it works?

It uses `__NV_PRIME_RENDER_OFFLOAD=1 __GLX_VENDOR_LIBRARY_NAME=nvidia [program]`.

`__NV_PRIME_RENDER_OFFLOAD=1` will cause the system to use Optimus/Prime technology.

`__GLX_VENDOR_LIBRARY_NAME=nvidia` will start any application with Nvidia GPU.

`[program]` can be any program, as long as it's OpenGL/Vulkan application.

*If you like it, consider giving a star.*
