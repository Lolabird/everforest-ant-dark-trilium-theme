# EverForest Ant Dark (EFAD) Trilium Theme
This is a [Trilium Notes](https://github.com/zadam/trilium) theme to go with Everforest and Ant Dark Linux desktop themes.

![Text Showcase](/screenshots/EFAD_Main.png)

## Features
### Native Styles
* Dark theme
* High contrast
* Scrolling tables with sticky headers on both axes
* Vertical floating buttons that have much less overlap with content of notes
* Custom fonts
* Earthy colors

### Enhanced Addon Styles
*See 'Usage Instructions' for information on how to enable these.*
* Zen Mode
* Matching syntax highlight in text notes
* Position shown in TOC
* And much more!

## Usage Instructions
* Download the latest version of Trilium
* Download the latest release of EverForest Ant Dark
* In your trilium instance right click a note you want to import the theme into
* Select "Import into note" in the context menu
* Uncheck "Safe import" and upload the zip file you just downloaded
* Click on the Trilium logo in the upper left corner and select Options -> Appearance
* Under "Theme", choose EverForest Ant Dark
* Enjoy!

### Enabling Addon Features
#### Zen Mode
* Create a 'JS frontend' code note
* Add the `#widget` attribute to 'Owned Attributes' (the button with three lines and a checkmark)
* Add the following code (created by [Nriver](https://github.com/Nriver/awesome-trilium/issues/44))) to the note
    ```js
    api.addButtonToToolbar({
        title: 'Zen mode',
        icon: 'spa',
        action: function() {
            $("body").toggleClass("zen-mode");
        },
        shortcut: 'alt+z'
    });
    ```
* Reload (`ctrl+r` or `F5`) Trilium to enable the script

##### Usage
Press `alt+z` or the zen (spa) button in the launcher (left most panel) to enable/disable zen mode.

There are two types of zen mode available:
1. Right panel enabled
2. Right panel disabled

Right panel is enabled by default. If you would like to disable it, you can either add the following code in a new CSS note or uncomment it in the Stellar Dark theme as seen in the video below.

```css
/*hide right pane*/
.zen-mode #right-pane {
    display: none !important;
}
```

https://github.com/user-attachments/assets/b4b12380-ea5b-4595-a65d-3189cc052a5d

##### Added Features
* Window control buttons are still accessible in zen mode
* Zen button is still accessible in zen mode for easy disabling in case you don't remember the shortcut
* Bottom panel widgets are not visible in zen mode
* Optional disabling of right panel in zen mode

#### Show Position in TOC and Syntax Highlight
Please go to each addon's respective page for instructions on how to enable these addons.
* [Show Position in TOC](https://github.com/SiriusXT/trilium-show-position-in-toc)
* [Syntax Highlight](https://github.com/antoniotejada/Trilium-SyntaxHighlightWidget)

## Screenshots and Videos
![Selection Showcase](/screenshots/EFAD_Hover.png)

https://github.com/user-attachments/assets/7b5a7857-972e-454f-b7c1-da93ac4840aa

![Map Showcase](/screenshots/EFAD_Map.png)

![Code Showcase](/screenshots/EFAD_Code.png)

https://github.com/user-attachments/assets/7c00d31c-a43e-4956-87f8-f5ce220088de

![Text Note Syntax Highlight Showcase](/screenshots/EFAD_Highlight.png)

## Credits and Resources
### Fonts
Jost: https://indestructibletype.com/Jost.html
JetBrainsMono: https://www.jetbrains.com/lp/mono/

### Desktop Themes
#### Ant Dark
KDE: https://store.kde.org/p/1464285/
GitHub: https://github.com/EliverLara/Ant/tree/master/kde/Dark

#### EverForest
*Note: There are several EverForest Firefox themes, but the one I personally like and use is listed below.*

* Gnome: https://www.gnome-look.org/p/1695467
* GitHub (Gnome): https://github.com/Fausto-Korpsvart/Everforest-GTK-Theme
* Firefox: https://addons.mozilla.org/en-US/firefox/addon/everforest_theme/

#### Zafiro Icon Theme
*Note: I only have GitHub and KDE listed below, but this set is also available for other desktop environments as well.*

* GitHub: https://github.com/zayronxio/Zafiro-icons
* KDE: https://store.kde.org/p/1209330

### Addons Featured in the Screenshots and Videos
* [Breadcrumbs](https://github.com/rauenzi/Trilium-Breadcrumbs)
* [Scratchpad](https://github.com/zadam/trilium/discussions/1613#discussioncomment-638984)
* [Show Position in TOC](https://github.com/SiriusXT/trilium-show-position-in-toc)
* [Syntax Highlight](https://github.com/antoniotejada/Trilium-SyntaxHighlightWidget)
* [Theme Switch](https://github.com/madodig/trilium-widget-theme-switch)
* [Trilium Chat](https://github.com/soulsands/trilium-chat)
* WordCount (Featured in the [Demo Document](https://github.com/zadam/trilium/wiki/Document#demo-document))
* [Zen Mode](https://github.com/Nriver/awesome-trilium/issues/44)

Find more addons made by the Trilium community at [Nriver's Awesome Trilium](https://github.com/Nriver/awesome-trilium?tab=readme-ov-file#%EF%B8%8F-widgets)!
