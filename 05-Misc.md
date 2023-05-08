**[ [Home](00-Home.html) | [Core](01-Core.html) | [Dialog](02-Dialog.html) | [Job](03-Job.html) | [Misc](05-Misc.html) | [Side](06-Side.html) | [View](07-View.html) | [Widget](08-Widget.html) | [Other](99-Other.html) ]**

## Misc

---

#### app_notify

* Description
    
    Functions to display notification messages such as unmount notifications.


#### ThunarBrowser
    
* Description

    A GInterface used by Application, LocationEntry and Launcher to
    resolve a file before launching it. For example, Application calls
    browser_poke_file to resolve a file given on the command line and
    then launch it in a callback using th_file_launch.


#### ThunarComponent

* Description

    A GInterface to store selected files. Launcher, TreePane and StandardView
    implement it.


#### ThunarHistory

* Description

    A GObject to handle back, forward browse history. ThunarHistory
    implements a ThunarNavigator interface.


#### IconFactory

* Description
    
    A GObject to cache icons and thumbnails.


#### IconRenderer

* Description
    
    A GtkCellRenderer to display TreeView and ListView icons.

* Shortcut arrow in Thunar
    
    Thunar renders shortcut arrows the same way as emblems.
    thunar_icon_renderer_render calls thunar_file_get_emblem_names which
    adds a symbolic link emblem name.
    
    ```
    if (thunar_file_is_symlink (file))
        emblems = g_list_prepend (emblems, THUNAR_FILE_EMBLEM_NAME_SYMBOLIC_LINK);
    ```


