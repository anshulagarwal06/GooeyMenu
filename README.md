
Option menu with gooey effects.


Inspired by this [dribbble](https://dribbble.com/shots/1936758-GIF-of-the-Tap-Bar-Concept):


![](dribble.gif)

### What this Lib can do :

**1.Tab on each menu you get call with menu number.**

**2.You can customize the number of the menu.**

**3.Distance between super menu and sub men can be customize.**

**4.Customize menu icon.**

![](gooeyeffect.gif)


also,you can set the menu's icon:

# Download

Include `jitpack.io` inside of **root** project `build.gradle`:

```groovy
allprojects {
		repositories {
			...
			maven { url "https://jitpack.io" }
		}
	}
```

After that you can easily include the library in your **app** `build.gradle`:

```groovy
dependencies {
	        compile 'com.github.anshulagarwal06:GooeyMenu:-SNAPSHOT'
	}
```

# Instructions

```groovy
    <com.anshul.gooey.GooeyMenu
        android:id="@+id/gooey_menu"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        app:center_menu_src="@drawable/logo_cardmap"
        app:fab_radius="@dimen/big_circle_radius"
        app:gap_between_menu_fab="@dimen/min_gap"
        app:gooey_colors="@array/color_array"
        app:menu_drawable="@array/drawable_array"
        app:menu_radius="@dimen/small_circle_radius"
        app:menu_visible_on_start="false"
        app:no_of_menu="4"/>
```

Most of xml attributes are self explanatory.  

- **no_of_menu** : Number of menu item in gooeyMenu
- **menu_visible_on_start** : default value is true. It control menu visibility on start.
- **menu_radius**  : menu item circle radius.
- **fab_radius_radius**  : Fab button radius.
- **fab_menu_src**  : Fab button drawable resource.
- **menu_drawable**  :drawable Array of menu items.

- **gooey_colors**: Color array of gooeymenu. First item in array is for Fab color, rest is for menu items.

That's it. build your project.