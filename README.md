# Four-Gtk-Theme
Gtk theme for linux of preferred use in Window Managers.  
This theme is a modification of the [Orchis](https://github.com/vinceliuice/Orchis-theme) theme,  
And many of the things it has by default have been removed, so that only the  
essential is left to be used in a window manager.

## Install
- Clone this repository..  

git clone https://github.com/cesarediego/Four-Gtk-Theme.git   
- Check if the ~/.themes directory exists.  
- If it doesn't exist, create it with mkdir ~/.themes  
- Copy the theme with:  

cp -r Four ~/.themes  

## How to customize?
Customizing this theme is very simple.  
Inside the theme directory in gtk-3.0, there are 4 files related to the theme.  
- (gtk.css) the main file  
- (colors.css) Contains the path that the main file will use.  
This file can be changed manually or in a highly customized script.  
- (dark.css) Contains dark color scheme  
- (light.css) Contains white color scheme  

To make modifications manually, you can modify the themes (dark and light), changing the colors that are contained in these files.  
The theme uses simple logic.  
  
> These are the accent colors.  
>> @define-color red #ef476f;  
>> @define-color yellow #e85d04;  
>> @define-color green #06d6a0;  
>> @define-color blue #118ab2;  
>> @define-color purple #c4a3d2;  
>> @define-color gray #8e9aaf;  
>> @define-color cyan #4cc9f0;  
>> @define-color magenta #ff006e;  
>    
>>> These are the base colors.  
>>>> /**** Background Colors ****/  
>>>> @define-color base #061115;  
>>>> @define-color base-alt #021216;  
>>>> /**** Text Colors ****/  
>>>> @define-color font #f5f5f5;  
>  
>>>> Use one of the accent colors to change this line.  
>>>>> /**** Highlight Colors *****/  
>>>>> @define-color highlight @blue;  
  
By changing this file the whole theme will be changed,  
use it carefully, do several tests with colors to find the one you like the most.  
  
If you want to create a script to change the theme from light to dark automatically, the command is:  
Light  
* echo '@import url("light.css");' > ~/.themes/Four/gtk-3.0/colors.css  
Dark
* echo '@import url("dark.css");' > ~/.themes/Four/gtk-3.0/colors.css  
With this command it is possible to create a simple script to be used by the terminal,  
or in a button on a bar like tint2, polybar, xfce4-panel...