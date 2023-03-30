# Creating a NoteSkin
---

Creating your own NoteSkin is relatively easy, if you're familiar with some of the same
	processes that people use to make skins on osu!. \
\
To get started, we'll copy out the NoteSkin `DivideByZero`.
	It's a good first start for anyone just learning how to make their own
	note design, or someone looking to port a NoteSkin over from another
	game. \
The `DivideByZero` NoteSkin is located in: \
`<The Etterna folder>/NoteSkins/dance/DivideByZero` \
\
> ![](info.png) \
> The Etterna folder is usually located at:
> - `C:\Windows\Games\Etterna` on Windows
> - `/opt/etterna` on Arch Linux
> - `~/.var/app/com.etternaonline.Etterna/data/gamedata` on [the Linux flatpak](https://github.com/kurulen/com.etternaonline.Etterna)
> - The folder for Etterna on macOS hasn't been added here, please consider
	[contributing.](https://github.com/kurulen/eac/pulls)

After you've copied it over, you'll be able to edit the images and Lua contained
	within, without fear of destroying the NoteSkin you copied it from. \
\
We'll start by editing the images, and we'll be using [GIMP](https://gimp.org) for right now. \
Open the image in GIMP, and you'll likely see what's known as a *spritesheet*.
	Spritesheets look like different images rolled into one, and that's
	exactly what they are. \
You'll be able to see how many images are in a spritesheet by looking at its
	filename, near the end. There will usually be something similar to `1x8`
	there, where 1 is the amount of columns in the image, and 8 is the
	amount of rows. \
For best results, you'll want to edit the images individually. You can use the
	spritesheet cutter linked in chapter 2 for this. \
After cutting the images in the spritesheet, you'll be able to edit them by
	yourself. To pack them back into an image, you'll likely need the
	texture packer linked in chapter 2. \
> ![](unstable_cliff.png) \
> You'll want to use the exact same column and row number
	as the original spritesheet for now, as the game will glitch out
	if you don't. \
> Additionally, depending on the direction the spritesheet went in
        (vertical or horizontal), you'll want to pack the textures back
        **in the exact same direction.** \

After packing the textures back how they originally were, you'll need to
	check if the resolution (both width and height) is a power of 2.
	Not doing this can lead to graphical glitches and errors. \
\
After that's complete, you can now save it over the spritesheet you originally
	used.
