---
title: UI Basics
description: This is intended to give you a summary of the EverQuest UI Engine used from 2002-2023
published: false
date: 2025-07-02T02:59:38.092Z
tags: ui guide
editor: markdown
dateCreated: 2025-06-14T06:20:39.026Z
---

[About SIDL](#about_sidl)

[Installer FAQ](#installer-faq)

[Discord](https://discord.com/invite/heroesjourney)

## EverQuest UI Basics

The EverQuest UI system is defined using **SUITE Interface Development Language (SIDL)**, an XML specification developed by Sony Online Entertainment and released in 2002, where various UI elements like windows, buttons, and animations are structured and linked. This allows for a modular and customizable interface.

To get help with the UI, join **The Heroes' Journey** community.

[Join the Discord](https://discord.com/invite/heroesjourney)

Check out our [Rules](/rules) before you start.

---

### The SIDL File Structure

The UI folder will have various different XML files, as well as texture files (.tga and .dds files). Most of the XML files will be related to a single interface window. There are a few exceptions to this:

-   **EQUI.xml** - This defines what xml files that the skin will use
-   **SIDL.xml** - This holds definitions for all of the individual elements and components
-   **EQUI\_Animations.xml** - This holds info on textures and how they are loaded into each component
-   **EQUI\_Templates.xml** - This defines templating for various elements, including texture references

The rest of the xml files will be named according to what UI element they create. Some examples are:

-   **EQUI\_Inventory.xml** - The Inventory screen. This is the most complex element and contains hundreds of components
-   **EQUI\_PlayerWindow.xml** - The player window
-   **EQUI\_TrackingWnd.xml** - The tracking window

  
All of your textures and miscellaneous other files will also be in the folder: 

-   **Images**
-   **Cursors**
-   **Target Indicators**

  
 

### Creating a Custom UI Skin

-   Go to the ***uifiles*** folder, located in your install directory
-   Make a copy of the ***default*** folder
-   Rename the copied folder. You cannot have spaces in the folder name

> The EverQuest client will not see the folder if there is a space in the name

![folder.png](/ui-page/folder.png)

-   Open your copied folder, you will see all of the files from the default skin
-   Find and open EQUI.xml (a custom tool is in development, but for now you can use [Notepad++](https://notepad-plus-plus.org/downloads/))

![equi1.png](/ui-page/equi1.png)

> You do not have to keep every file in your folder. The client will use elements from the default skin to fill in the gaps automatically

-   In this file, you set what your custom skin is going to load. Unless you are creating an entirely brand new skin, you can safely remove any entries here that you will not need
-   Make sure you leave the line that has SIDL.xml
-   Make sure you remove entire lines including the `Include` and `/Include` tags

### Button

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Style\_Checkbox | bool |     | This button acts as a checkbox (does not pop back up on mouse release) |
| RadioGroup | string |     | This button is part of a radio group. |
| Text | string |     | Text |
| ButtonDrawTemplate | ButtonDrawTemplate |     | Template that defines this button's art |
| SoundPressed | string |     | Sound to play on button press (currently not implemented) |
| SoundUp | string |     | Sound to play on button release (currently not implemented) |
| SoundFlyby | string |     | Sound to play on button hover (currently not implemented) |
| DecalOffset | Point |     | Offset for this button's decal, if it exists (see ButtonDrawTemplate) |
| DecalSize | Size |     | Size to fit this button's decal in, if it exists (see ButtonDrawTemplate) |

### ButtonDrawTemplate

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Normal | Ui2DAnimation:item |     | Image for a button just sitting around |
| Pressed | Ui2DAnimation:item |     | Image for a button under the oppression of the mouse click |
| Flyby | Ui2DAnimation:item |     | Image for a button with the mouse hovering over it |
| Disabled | Ui2DAnimation:item |     | Image for a button that has been disabled |
| PressedFlyby | Ui2DAnimation:item |     | Image for a depressed button with the mouse hovering over it (used by Checkbox buttons) |
| NormalDecal | Ui2DAnimation:item |     | Image that appears on top of a button |
| PressedDecal | Ui2DAnimation:item |     | Image that appears on top of a pressed button (defaults to NormalDecal if not set) |
| FlybyDecal | Ui2DAnimation:item |     | Image that appears on top of a highlighted button (defaults to NormalDecal if not set) |
| DisabledDecal | Ui2DAnimation:item |     | Image that appears on top of a disabled button (defaults to NormalDecal if not set) |
| PressedFlybyDecal | Ui2DAnimation:item |     | Image that appears on top of a disabled and highlighted button (defaults to NormalDecal if not set) |

### Class

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| item | string |     | Name that can be used to refer to this SUITE piece |

### ComboBox

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Button | ButtonDrawTemplate:item |     | Pull-down list button |
| ListHeight | int |     | Max height of this window when it is being pulled down |
| Choices | string\[\] |     | String choices to go into this combobox's pulldown list |

### Control

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Style\_VScroll | boolean | false | This control is vertically scrollable |
| Style\_HScroll | boolean | false | This control is horizontally scrollable |
| Style\_Transparent | boolean | false | You can see through this control |
| Style\_Border | boolean |     | This widget is surrounded by a border |
| TooltipReference | string |     | Help text for this control if the user holds the cursor over the item |
| DrawTemplate | WindowDrawTemplate:item |     | Template that defines this window's art |

### Editbox

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Style\_Multiline | boolean |     | This editbox can contain multiple lines of text |

### Frame

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Texture | string |     | Image texture this frame's image is contained in |
| Location | Point |     | Location of this frame's image in the texture |
| Size | Size |     | Size of this frame's image |
| Hotspot | Point |     | An important refrence point. For example, it is used to keep an animation centered if every frame in it is a variable size. This value is also used in cursors. |
| Duration | int | 1000 | Milliseconds of life for this frame in an animation cycle |
| Shading | RGB\[\] |     | A layer of shade to apply to the texture |
| Specular | RGB\[\] |     | A layer of specular gloss to apply to the texture |

### FrameTemplate

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| TopLeft | Ui2DAnimation:item |     | Image for this frame's top-left corner |
| Top | Ui2DAnimation:item |     | Image for this frame's top border |
| TopRight | Ui2DAnimation:item |     | Image for this frame's top-right corner |
| RightTop | Ui2DAnimation:item |     | Image for this frame's right-top border |
| Right | Ui2DAnimation:item |     | Image for this frame's right border |
| RightBottom | Ui2DAnimation:item |     | Image for this frame's right-bottom border |
| BottomRight | Ui2DAnimation:item |     | Image for this frame's bottom-right corner |
| Bottom | Ui2DAnimation:item |     | Image for this frame's bottom border |
| BottomLeft | Ui2DAnimation:item |     | Image for this frame's bottom-left corner |
| LeftTop | Ui2DAnimation:item |     | Image for this frame's left-top border |
| Left | Ui2DAnimation:item |     | Image for this frame's left border |
| LeftBottom | Ui2DAnimation:item |     | Image for this frame's left-bottom border |
| Middle | Ui2DAnimation:item |     | Image for this frame's center area |
| OverlapLeft | int | 0   | Pixels to let the middle overlap over the left frame |
| OverlapTop | int | 0   | Pixels to let the middle overlap over the top frame |
| OverlapRight | int | 0   | Pixels to let the middle overlap over the right frame |
| OverlapBottom | int | 0   | Pixels to let the middle overlap over the bottom frame |

### Gauge

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| GaugeDrawTemplate | GaugeDrawTemplate |     | Template that defines the art for this gauge |
| EQType | int |     | Defines what EQ value the gauge displays (HP, Mana, etc.) |
| FillTint | RGB |     | Color of the bar that fills in. |
| DrawLinesFill | boolean |     | Whether or not to draw the lines filling in |
| LinesFillTint | RGB |     | Color of the lines when filling in |
| TextOffsetX | int | 0   | X-offset for the text associated with this gauge |
| TextOffsetY | int | 0   | Y-offset for the text associated with this gauge |
| GaugeOffsetX | int | 0   | X-offset for the gauge itself |
| GaugeOffsetY | int | 16  | Y-offset for the gauge itself |

### GaugeDrawTemplate

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Background | Ui2DAnimation:item |     | Background image for the gauge |
| Fill | Ui2DAnimation:item |     | The bar that fills in on the gauge |
| Lines | Ui2DAnimation:item |     | The hash marks and hi-lites |
| LinesFill | Ui2DAnimation:item |     | The filled in version of the lines |
| EndCapRight | Ui2DAnimation:item |     | Right end cap piece |
| EndCapLeft | Ui2DAnimation:item |     | Left end cap piece |

### InvSlot

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| EQType | int |     | Inventory slot type (user, trading, merchant, bank, etc.) |
| Background | Ui2DAnimation:item |     | Background image for this inventory slot, when empty |
| ItemOffsetX | int | 0   | X-offset to apply to a contained item |
| ItemOffsetY | boolean | 0   | Y-offset to apply to a contained item |

### Label

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| NoWrap | boolean | false | Don't allow this label's text to wrap |
| AlignCenter | boolean | false | Center the text. By default, the text is left-justified |
| AlignRight | boolean | false | Right-justify the text. If AlignCenter is true, this value is ignored. |

### Listbox

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Columns | ListboxColumn\[\] |     | Columns that make up this listbox |
| OwnerDraw | boolean |     | This object draws its columns itself |

### ListboxColumn

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Header | FrameTemplate:item |     | A special frame for the heading of this list's column |
| Heading | string |     | The text for the heading of the list's column |
| Width | int |     | Width of this column |
| Sortable | boolean |     | Specifies if this list be sortable |
| DataType | string |     | Not used |

### Page

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| TabText | string |     | Text to attach to the tab that opens this page |
| TabIcon | Ui2DAnimation:item |     | Icon to attach to the tab that opens this page. The icon is always drawn left-justified. If any text also exists, it will be drawn to the right of the icon. |
| Pieces | ScreenPiece:item\[\] |     | Children items |

### Point

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| X   | int | 0   | X-coordinate |
| Y   | int | 0   | Y-coordinate |

### RGB

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Alpha | int | 255 | Transparency value, 0 - 255 |
| R   | int | 0   | Red value, 0 - 255 |
| G   | int | 0   | Green value, 0 - 255 |
| B   | int | 0   | Blue value, 0 - 255 |

### Screen

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Style\_Titlebar | boolean |     | True if this window has a titlebar |
| Style\_Closebox | boolean |     | True if this window has a close button |
| Style\_Minimizebox | boolean |     | True if this window has a minimize button |
| Style\_Sizeable | boolean |     | True if this window can be resized |
| Pieces | ScreenPiece:item\[\] |     | Children items |

### ScreenPiece

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| ScreenID | string |     | An identifier that is unique on the scope of all items being created within a parent control. All parent controls can access any of their children by this ID. |
| Font | int | 3   | Font style from 0 - 6 (0 being small, 6 being large) |
| RelativePosition | boolean | true | Draw this @ (x, y) relative from its parent window's topleft corner |
| Location | Point |     | (x, y) coordinates of top-left corner. Ignored if RelativePosition AND Autostretch is true. |
| Size | Size |     | (w, h) of item. Ignored if RelativePosition AND Autostretch is true. |
| AutoStretch | boolean | false | Stretch this window to the borders of its parent. If true, this window will be resized when his parent is resized. If not, all anchor variables (below) are ignored. |
| TopAnchorToTop | boolean | true | If true, keep the top side of this window a fixed offset away from its parent's top. Else, keep it a fixed offset away from its parent's bottom. |
| BottomAnchorToTop | boolean | true | If true, keep the bottom side of this window a fixed offset away from its parent's top. Else, keep it a fixed offset away from its parent's bottom. |
| LeftAnchorToLeft | boolean | true | If true, keep the left side of this window a fixed offset away from its parent's left. Else, keep it a fixed offset away from its parent's right. |
| RightAnchorToLeft | boolean | true | If true, keep the right side of this window a fixed offset away from its parent's left. Else, keep it a fixed offset away from its parent's right. |
| TopAnchorOffset | int | 0   | Used by TopAnchorToTop |
| BottomAnchorOffset | int | 0   | Used by BottomAnchorToTop |
| LeftAnchorOffset | int | 0   | Used by LeftAnchorToLeft |
| RightAnchorOffset | int | 0   | Used by RightAnchorToLeft |
| Text | string |     | Main text for this item. |
| TextColor | RGB |     | Color of the main text |

### ScrollbarDrawTemplate

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| UpButton | ButtonDrawTemplate |     | Template that defines the art for this scrollbar's up button |
| DownButton | ButtonDrawTemplate |     | Template that defines the art for this scrollbar's down button |
| Thumb | FrameTemplate |     | Template that defines the art for this scrollbar's scroll box |
| MiddleTextureInfo | string |     | Filename for an image file whose entirety is the pattern for for the scroll area of the scrollbar |
| MiddleTint | RGB |     | Tint to apply to the scroll area texture |

### Size

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| CX  | int |     | Width value |
| CY  | int |     | Height value |

### Slider

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| SliderArt | SliderDrawTemplate:item |     | Template that defines the art for this slider |

### SliderDrawTemplate

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Thumb | ButtonDrawTemplate |     | Template that defines the art for this slider's thumb (the piece that is scrolled to change the slider's value) |
| Background | Ui2DAnimation:item |     | Background image for the slider (that the thumb scrolls along) |
| EndCapRight | Ui2DAnimation:item |     | Right end cap piece |
| EndCapLeft | Ui2DAnimation:item |     | Left end cap piece |

### SpellGem

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| SpellGemDrawTemplate | SpellGemDrawTemplate |     | Template that defines the art for this spellgem |
| SpellIconOffsetX | int | 0   | Offset of the icon onto this spellgem's background |
| SpellIconOffsetY | int | 0   | Offset of the icon onto this spellgem's background |

### SpellGemDrawTemplate

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Holder | Ui2DAnimation:item |     | The image for the spell gem container (when empty) |
| Background | Ui2DAnimation:item |     | The background for a spell gem icon |
| Highlight | Ui2DAnimation:item |     | A shine to put on the spellgem on mouseover |

### StaticAnimation

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Animation | Ui2DAnimation:item |     | An animation to draw |

### StaticFrame

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| FrameTemplate | FrameTemplate:item |     | A frame to draw |

### StaticHeader

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| FrameTemplate | FrameTemplate:item |     | A header frame to draw that has some text in it (useful for a menu) |
| TextReference | string |     | The text to draw |
| TextColor | RGB |     | The text color to draw with |

### StaticScreenPiece

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| AutoDraw | boolean | true | Have this piece automatically appear (as opposed to having the code programmatically choose to draw it) |

### StaticText

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| NoWrap | boolean | false | Don't allow this text to wrap if squished |
| AlignCenter | boolean | false | Center this text |
| AlignRight | boolean | false | Right justify this text |

### STMLbox

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| No specific parameters listed in the provided data. \[cite\_start\]This is a read-only text area that displays STML (a subset of HTML), allowing for color, font size variations, etc. \[cite: 41\] |     |     |     |

### SuiteDefaults

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| DefaultWindowDrawTemplate | WindowDrawTemplate:item |     | Store the game's standard window |
| CursorDefault | Ui2DAnimation:item |     | Default cursor |
| CursorResizeNS | Ui2DAnimation:item |     | Default (( cursor |
| CursorResizeEW | Ui2DAnimation:item |     | Default (( cursor |
| CursorResizeNESW | Ui2DAnimation:item |     | Default (( cursor |
| CursorResizeNWSE | Ui2DAnimation:item |     | Default (( cursor |
| CursorDrag | Ui2DAnimation:item |     | Default cursor when dragging an item |

### TabBox

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| TabBorderTemplate | FrameTemplate:item |     | The template that defines the art for a tab |
| PageBorderTemplate | FrameTemplate:item |     | The template that defines the art for the main window frame where each tab page goes. |
| Pages | Page:item\[\] |     | A collection of pages (each page gets an associated tab). |

### TextureInfo

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Size | Size |     | The size of this image file |

### Ui2DAnimation

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Cycle | boolean |     | Cycle the animation |
| Grid | boolean |     | Set this animation to be a grid (used for drag items, etc.) |
| Vertical | boolean |     | Grid is Vertical instead of horizontal (only used when Grid = true) |
| CellHeight | boolean | 0   | Height of each cell in the grid (only used when Grid = true) |
| CellWidth | boolean | 0   | Width of each cell in the grid (only used when Grid = true) |
| Frames | Frame\[\] |     | Animation frames |

### WindowDrawTemplate

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| Background | TextureInfo:item |     | Background image for this window |
| VSBTemplate | ScrollbarDrawTemplate |     | Template that defines this window's vertical scrollbar art |
| HSBTemplate | ScrollbarDrawTemplate |     | Template that defines this window's vertical scrollbar art |
| CloseBox | ButtonDrawTemplate |     | Template that defines this window's close button art |
| MinimizeBox | ButtonDrawTemplate |     | Template that defines this window's minimize button art |
| TileBox | ButtonDrawTemplate |     | Template that defines art to tile all along this window's background |
| Border | FrameTemplate |     | Template that defines this window's border art |
| Titlebar | FrameTemplate |     | Template that defines this window's title art |