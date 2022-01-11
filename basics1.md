# DA BASICS
### Let's start off with sprites...
There are special functions that will help you with adding/removing sprites, such as:
## makeLuaSprite(tag:String, image:String, x:Float, y:Float)
Spawns a Lua Sprite with no animations using the tag `tag`, it will be using the image `image`.png, and will be spawned on position `x`, `y` If you want to make a Black screen with no texture, leave `image` field empty and use (luaSpriteMakeGraphic)[]

If another Lua Sprite that exists is already using the tag `tag`, it will be removed.
## And now for animated sprites!
In case you want to make an animated sprite:
## makeAnimatedLuaSprite(tag:String, image:String, x:Float, y:Float)
Spawns a Lua Sprite that supports Animations, it will be using the tag `ta`g, be using the image `image`.png, the XML `image`.xml, and will be spawned on position `x`, `y`

If another Lua Sprite that exists is already using the tag `tag`, it will be removed.

## Just some reminders
1. If you want to add a sprite, there is a separate function called **addLuaSprite(tag:String, front:Bool = false)**.
2. The same goes for **removeLuaSprite(tag:String, destroy:Bool = true)**, except it removes sprites instead of adding them
3. These can be really useful for custom stages!

# CUSTOM TEXT
### Moving on to Custom Text
Just like helpers with adding/removing sprites, there's also ones for text, too:

## makeLuaText(tag:String, text:String, width:Int, x:Float, y:Float)
creates a Lua Text object on position `x`, `y` and a width with 'width'

## Some more reminders
1. You can add/remove using separate functions, too
2. These can be useful if you want to make a mechanic of some sorts involving score and other stuff
3. You can set nearly every property of text as a bonus
