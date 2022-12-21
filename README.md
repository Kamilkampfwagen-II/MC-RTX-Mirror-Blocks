# MC-RTX-Mirror-Blocks
**THIS PACKS NEEDS DXR ENABLED TO WORK AS INTENDED. WITHOUT RAY TRACING NEW TEXTURES WILL APPEAR WHITE**\
Resource packs retexture following:
- White glass
- Activator rail

I've chosen those because they are not really common in builds.

**Some Tips:**
- Both sides of the activator rail have the same mirror texture. This enables following:
- You can build a working periscope. Rail slope is 45 degrees.
- To place rails in the air *-you obviously need to build a 2x2 stair-*, use barrier blocks. In case of glass blocks:


[light source] -> [glass] -> [rail] -> [glass] -> [rail] -> [camera]


As you can see, light will have to pass through two separate glass blocks in order to reach to the bottom.


For some reason, this removes the color information of entities. This includes everything handled by Entity Model Renderer like chests, beds etc.
- Light bounce limit is 8.

**How to Create Your Own:**
If you are not happy with my choices, you can use the template to create a new one yourself.
- Download the repository: Code -> Download ZIP
- Go to **Template/Textures/Blocks**
- Duplicate the **block_texture.texture_set.json** file if you need to retexture multiple blocks in a single package
- All textures that can be turned into mirrors are specified in **TextureList.txt** _If you see mistakes please create an issue_
- Grab a texture name from the list. Keep in mind that subblocks use the same texture as their type. (stairs-slabs etc use their plank texture)
- Rename each **block_texture.texture_set.json** file to **TEXTURE NAME YOU JUST GRABBED FOR THAT BLOCK.texture_set.json**
- Go back to the Template folder
- Open up manifest.json with notepad
- Edit description and name whatever you want but don't mess up with quotes
- Open up the link in the next line and generate a random UUID. Change the value of the line with that UUID. If you don't have an internet connection, open up one of the .mcpack files as ZIP, copy its UUID then change some random numbers and use that.
- The same step goes for the other UUID, never use the same UUID twice
- Change version info if you want
- Save the file
- Replace **pack_icon.png** if you want. It should be a square to be displayed correctly. Max resolution is **1080x1080** but lower is recommended. Otherwise, it will waste disk space
- Add everything to a **zip** file
- Change the file extension to **mcpack**

**Congratulations!** You have just created your very own resource pack.
