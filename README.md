# EVERQUEST CLASSIC ART MODS
fan art modifications in everquest classic 

| [DOWNLOAD MOD]( https://github.com/CorvaeOboro/everquest_art_mods/releases/download/everquest_art_mods_20231117/everquest_art_mods_innothule_grobb_20231117.zip)    |   [VIEW IMAGES]( https://corvaeoboro.github.io/everquest_art_mods/everquest_art_mods_all.htm )   |    [DOWNLOAD SOURCE]( https://github.com/CorvaeOboro/everquest_art_mods/archive/refs/heads/main.zip ) | 

# Install 
backup then replace zone .s3d files in EverQuest folder ( p99 and quarm tested ) . 

# Innothule + Grobb 
![everquest_art_mods_header_innothulegrobb](https://raw.githubusercontent.com/CorvaeOboro/everquest_art_mods/master/docs/everquest_art_mods_header_innothule_grobb.jpg?raw=true "everquest_art_mods_header_innothulegrobb")


![everquest_art_mods_unreal_render_gif](https://raw.githubusercontent.com/CorvaeOboro/everquest_art_mods/master/docs/everquest_art_mod_unreal_20231117.gif?raw=true "everquest_art_mods_unreal_render_gif")


https://github.com/CorvaeOboro/everquest_art_mods/assets/6800097/97151377-990b-433a-a888-f2e495b26c21


https://github.com/CorvaeOboro/everquest_art_mods/assets/6800097/27690ab9-f65f-475f-a418-1acd7d2e9605


# Notable changes 
- water stilled , meat removed 
- writing altered to Trollish from TrollHunters by Guillermo del Toro

# Process 
Import/Export
- export textures from zones .s3d files using EQZIp 
- export mesh as obj using S3D Zone Exporter ( exports the entire zone including placed object instances , however some objects have incorrect positioning )
- import textures into .s3d files using EQZIp

153 textures synthesized , 49 removed , 25 hidden
- upscale ( swinir ) 
- paintover + photo collage + filterforge
- stable diffusion ( controlnet + asymmetric tiling ) 
- adobe generative fill ( inpainting fixes )

Texture Format  
- using texconv in python to convert the PSD to DDS , then renamed to BMP to match the existing files ( importing without auto dds conversion as DXT1 , for mipmap support , and flipping vertically )
- textures with opacity are saved to tga , then imported into EQZIP with the option to convert imports to DDS in the preferences set to 16bit .

Hidden
- a number of objects have been hidden by changing their material to transparent and texture set to zero opacity . 
- using the [WLD Suite Transparentifier](https://docs.eqemu.io/server/zones/customizing-zones/wld-editor-suite/#instructions_1)
- hidden objects : meat , butcherblock rock , chain hook , metal spheres , throne grunge

# Thanks
- many thanks to everquest community creating emulators , tools , and content !
- LanternEQ - LanternExtractor - [https://github.com/LanternEQ/LanternExtractor](https://github.com/LanternEQ/LanternExtractor)
- Shendare - EQZip - [https://github.com/Shendare/EQZip](https://github.com/Shendare/EQZip)
- Zaela - WLD Suite - [https://github.com/Zaela](https://github.com/Zaela)
- EQemu - Wiki + Tools [http://www.eqemulator.org/](http://www.eqemulator.org/)
- Xackery - Quail - [https://github.com/xackery/quail](https://github.com/xackery/quail)

# License
- Everquest is a registered trademark of Daybreak Game Company LLC.  
- this art mod is not associated or affiliated in any way with Daybreak Game Company LLC.
- none of the original textures are included , all have been replaced or removed .
- all textures are free to all , [creative commons CC0](https://creativecommons.org/publicdomain/zero/1.0/) , free to re-distribute , attribution not required
