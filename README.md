**Update 2020**

Got warning from github about my location, [https://gitlab.com/danilw](https://gitlab.com/danilw) is mirror when this github account will be banned.

**update 2019**

gitlab mirror [https://gitlab.com/danilw](https://gitlab.com/danilw), untill I can update github repo I will (depends of github rules(region block) updates based on U.S. laws)

# godot-utils-and-other
**what is it** random(mosly some very broken demos, and very unusable utils) code I write using Godot. I do not recoment use this code for learning.

### Contact: [**Join discord server**](https://discord.gg/JKyqWgt)


*new 2020:*
___

**portals_panorama** GLES2 scene with six very simple **procedural panorama** for godot. Shader source code in [panorama/shaders](https://github.com/danilw/godot-utils-and-other/tree/master/portals_panorama/panorama/shaders) folder.

Video [youtube link](https://youtu.be/GyX0rkKkdFU)

*links* **[Live web build](https://danilw.github.io/godot-utils-and-other/portal_panorama/web/portals_panorama.html)**, [Win64](https://danilw.github.io/godot-utils-and-other/portal_panorama/portal_panorama_win.zip), [Linux64](https://danilw.github.io/godot-utils-and-other/portal_panorama/portal_panorama_linux.zip)

*Support*: Godot 3.1, Godot 3.2, GLES2 or GLES3. Used official Godot build, nothing else.

**How yo use** in your project: create MeshInstance, mesh Sphere, in mesh check *flip faces*, create shader material, in shader code copy-paste any of *\*.shader* code form this project. (for advanced use look this project source)

**Portals** they are *bad*, they exist only for this demo-scene. Portals rendered with *huge-overhead* because Light Cull Mask [not implemented](https://github.com/godotengine/godot/issues/19438) in Godot 3.x versions.

*Used external resources*: I have use external resources, [list of used 3d models](https://github.com/danilw/godot-utils-and-other/blob/master/portals_panorama/resources/using_external_resources_LINKS.md), and original shader-source linked in each *\*.shader* file.

*Licence* of shaders License Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License.
___

*old 2019:*
___

**flat-maze** demo base on particle collision, that show more complex collisions. link to repo https://github.com/danilw/flat-maze playable web version **https://danilw.itch.io/flat-maze-web**

Video [youtube link](https://youtu.be/HawWnuMn1mc)
___

**particle_self_collision** very simple GPU collision for thousands **Indexed**-*particles*, each particle with own index and other unique data, on GLES3/WebGL2, using Godot. [**live(web) demo link**](https://danilw.github.io/godot-utils-and-other/particle_self_collision/minimal_example/web_demo/mini_example.html) , or download for [Win64(exe)](https://danilw.github.io/godot-utils-and-other/particle_self_collision/minimal_example/particles_collision_win.zip)

this is GLSL-only logic, example on shadertoy https://www.shadertoy.com/view/tstSz7

Video [youtube link](https://youtu.be/fRu9PA4XHPQ)

**Building:** you need rebuild Godot with enabled `GL_RGBA32F` suport, read this page [**there building howto**](https://github.com/danilw/flat-maze)
___

**Menu_2DGI** rendering static textures and use them as menu textures, include render and examples.
To edit *max number of shapes* (is 5) edit `const max_elems` in scene.gd, and `int max_elems` in 2dGI.shader. (used default Godot 3.1.1)

How to use [watch video](https://youtu.be/HTuG5UOMC74).

**Web version**, live **Examples**: [Smooth color](https://danilw.github.io/godot-utils-and-other/menu_2DGI/example_3/web/example_3.html) example. *Minimal* examples [1](https://danilw.github.io/godot-utils-and-other/menu_2DGI/example_1/web/example_1_minimal.html) [2](https://danilw.github.io/godot-utils-and-other/menu_2DGI/example_2/web/example_2_text.html).

Download *bin*:**Render** for [Windows](https://danilw.github.io/godot-utils-and-other/menu_2DGI/editor/menu_2D_GI_editor_win.zip) or [Linux](https://danilw.github.io/godot-utils-and-other/menu_2DGI/editor/menu_2D_GI_editor_linux.zip). **Examples** example [1](https://danilw.github.io/godot-utils-and-other/menu_2DGI/menu2DGI_examples_bin/menu2DGI_example_1.zip), [2](https://danilw.github.io/godot-utils-and-other/menu_2DGI/menu2DGI_examples_bin/menu2DGI_example_2.zip), [3](https://danilw.github.io/godot-utils-and-other/menu_2DGI/menu2DGI_examples_bin/menu2DGI_example_3.zip)
___

**e-ani** link to repo with source code https://github.com/danilw/e-ani playable version download from https://danilw.itch.io/e-ani
___

**a_rel_bw_game** *Warning: code very bad!* || Using lots of particles in Godot, in small demo-game.
To build this project you need build Godot with module **futari-addon** (google it(gitlab) ot use this [link](https://gitlab.com/polymorphcool/futari-addon) ) *Binary versions*: [win64](https://danilw.github.io/godot-utils-and-other/a_rel_bw_game/bw_game_win64.zip) [linux64](https://danilw.github.io/godot-utils-and-other/a_rel_bw_game/bw_game_lin64.zip) [live/web](https://danilw.github.io/godot-utils-and-other/a_rel_bw_game/web/afg.html)(work only in Firefox [reason](https://github.com/godotengine/godot/issues/28573)) (native builds have Mipmap On, web build off)
___

**Dynamic sky and reflection** two shaders for sky and reflection [video](https://youtu.be/IQ-yw19xBQ8), [live link](https://danilw.github.io/godot-utils-and-other/dyn_sky_refl/web/dsr.html) and [windows version](https://danilw.github.io/godot-utils-and-other/dyn_sky_refl/bin/win.zip)

**Environment bug**(on first load): Godot has bug with removing *Default Environment* after re-import Assets(project is work if launch, it does not work only in Godot editor), set Project->Projet Setting->Rendering->Environment->Default Environment select file *default_env.tres*
___

*new small:*

**2d_ex_physics** simply(100 lines of code) circle collision with gravity on GDScript, from my [old project](https://youtu.be/lVCIEaFEMO4), check [video](https://youtu.be/zOYQ6vljZSI) and [live_web](https://danilw.github.io/godot-utils-and-other/2d_ex_physics/web/2d_ex_physics.html)

2d explossion effects [video](https://youtu.be/h7C2-YMFn94) [src1](https://danilw.github.io/godot-utils-and-other/2d_explossions/explossion_no_bb.zip) [src2](https://danilw.github.io/godot-utils-and-other/2d_explossions/explossion_with_backbuffer_ex.zip) [live1](https://danilw.github.io/godot-utils-and-other/2d_explossions/web/no_fb_v0/explossion_with_backbuffer_ex.html) [live2](https://danilw.github.io/godot-utils-and-other/2d_explossions/web/feedback_v1/explossion_with_backbuffer_ex.html)
___

*old:*

**Godot_shadertoy** very simple "Shadertoy logic to Godot" [video](https://youtu.be/v48O7Nk_n4g), [source repo](https://github.com/danilw/GLSL-howto/tree/master/Godot_shadertoy)

**Cubemap to panorama** convertor [live link](https://danilw.github.io/GLSL-howto/cubemap_to_panorama_js/cubemap_to_panorama.html) 

**Godot-particles-collision** *unfinished* particle collision shader for Godot [source repo](https://github.com/danilw/Godot-particles-collision)



### Graphic

**portals_panorama** video
[![pp](https://danilw.github.io/godot-utils-and-other/portal_panorama/yt.png)](https://youtu.be/GyX0rkKkdFU)


**Particle-collision-demo** (flat-maze game) video:
[![flat_maze](https://danilw.github.io/godot-utils-and-other/flat_maze_yt.png)](https://youtu.be/HawWnuMn1mc)


**Menu_2DGI** video(click)

[![Menu_2DGI](https://danilw.github.io/godot-utils-and-other/menu_2DGI/2dgi_yt.jpg)](https://youtu.be/HTuG5UOMC74)

**e-ani** video 

[![e-ani](https://danilw.github.io/godot-utils-and-other/yt_e-ani.png)](https://youtu.be/0jKyTBFrpjU)


**a_rel_bw_game** video

[![a_rel_bw_game](https://danilw.github.io/godot-utils-and-other/a_rel_bw_game/bw_game_yt.jpg)](https://youtu.be/jTmppCifnYE)

**Dynamic sky and reflection**

![dyn](https://danilw.github.io/godot-utils-and-other/dyn_sky_refl/dsr.jpg)
