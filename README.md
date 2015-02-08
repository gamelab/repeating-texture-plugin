====================

- Name: Repeating Texture Plugin.
- Version: 1.1
- Type: GameObject Plugin
- Author: Kiwi.js Team
- Website: www.kiwijs.org
- Kiwi.js Version Last Tested: 1.1.1


##Versions

1.0 - Initial GameObject created.


##Description:

Repeating Texture is a Plugin for Kiwi.js that gives you access to a new GameObject which is used for displaying repeating textures within an area. 

Note that this particular GameObject isn't designed to be used for applications like CollisionDetection but more for basic repeating background, so you don't have to always use multiple sprites. 

If you have any problems then feel free to contact us via the http://www.kiwijs.org/help


##How to Include: 

**First Step:**
Copy either the repeating-texture-[version].js or the repeating-texture-[version].min.js file (they should be right next to this one right now) into your project directory. We recommend that you save the files under a plugin directory that lives inside of your project directory so that you can easily manage all of the plugins but that is not required.


**Second Step:**
Link in the JavaScript file (repeating-texture-[version].js or the min version of the file) into your HTML file. Make sure you link it in underneath the link to the main Kiwi.js file AND underneath the Cocoon files.


##How to use.

**Take Note!**

- Rotation or Scale has not been tested and may not function as wanted/intended. Use at own discretion. 

##Creating a new Object

To create a new RepeatingTexture GameObject all you have to do is instate the GameObject and add it as a child to a State (just like any normal Sprite/StaticImage).

```
var bg = new Kiwi.Plugins.GameObjects.RepeatingTexture(this, this.textures.yourTextureAtlasName, xCoordinate, yCoordinate, widthOptional, heightOptional);
this.addChild(bg);
```

If you don't want the image to be repeatly rendered on a particular axis's, then you can set the 'repeatX' or 'repeatY' properties to 'false' on the RepeatingTexture GameObject.

```
bg.repeatX = false; //Stops repeating on the x-axis.  
bg.repeatY = false; //Stops repeating on the y-axis.
```

