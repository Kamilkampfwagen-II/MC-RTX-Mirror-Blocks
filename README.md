# MC-RTX-Mirror-Blocks
**THIS PACKS NEEDS DXR ENABLED TO WORK AS INTENDED. WITH RAY TRACING OFF THEY WILL APPEAR WHITE**\
Resource packs to convert some vanilla blocks into mirrors.

- Mirror textured white glass
- Mirror textured activator rail

I chose those blocks to retexture because they are the least common blocks suitable for this purpose as the way I see it.

**Some Tips:**
- Both sides of the activator rail have the same mirror texture. For those of you wondering.
- With mirror textured rails, you can build a working periscope. Their slope is exactly 45 degrees so they reflect the direct light at exactly 90 degrees.
- To place them in the air you can use either glass or a barrier block. You may need a borderless glass block addon. For some reason, color information on entity models gets lost when passing through two different glass blocks or the same with a gap between them. You won't be able to see the colors of things handled by entity model renderer like mobs, chests, etc. To avoid this, use a barrier block instead. It has no refraction.
- MC RTX's light bounce limit is 7; if you are looking into a chain of mirrors, the rest will appear gray. Mirrors rooms will have 14 reflections per dimension.

**How to Create Your Own:**
If you are not happy with my choices, you can use the template to create one yourself.
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
- The same step goes for the other UUID, never use the same UUID again
- Change version info if you want
- Save the file
- Replace **pack_icon.png** if you want. It should be a square to be displayed correctly. Max resolution is **1080x1080** but lower is recommended. Otherwise, it will waste disk space
- Add everything to a **zip** file **NOT RAR OR 7Z**
- Change the file extension to **mcpack**

**Congratulations!** You have just created your very own mirror resource pack.
