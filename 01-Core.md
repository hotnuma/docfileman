**[ [Home](00-Home.html) | [Core](01-Core.html) | [Dialog](02-Dialog.html) | [Job](03-Job.html) | [Misc](05-Misc.html) | [Side](06-Side.html) | [View](07-View.html) | [Widget](08-Widget.html) | [Other](99-Other.html) ]**

## Core

---

#### Modules
    
* ThunarFile
    
    ```
    GObject
    ╰── ThunarFile
    ```
    
    :973:thunar_file_info_reload.c

    ```
    file->collate_key = g_utf8_collate_key_for_filename (file->display_name, -1);
    ```
    
    :4144:thunar_file_compare_by_name


* ThunarClipboardManager
    
    ```
    GObject
    ╰── ThunarClipboardManager
    ```
    
    ```
    thunar/thunar-launcher.c:1308:  ThunarClipboardManager   *clipboard;
    thunar/thunar-launcher.c:2560:  ThunarClipboardManager *clipboard;
    thunar/thunar-launcher.c:2577:  ThunarClipboardManager *clipboard;
    thunar/thunar-launcher.c:2594:  ThunarClipboardManager *clipboard;
    thunar/thunar-launcher.c:2608:  ThunarClipboardManager *clipboard;
    thunar/thunar-icon-renderer.c:379:  ThunarClipboardManager *clipboard;
    thunar/thunar-tree-view.c:181:  ThunarClipboardManager *clipboard;
    thunar/thunar-window.c:304:  ThunarClipboardManager *clipboard;
    ```







* ThunarUserManager

    https://developer.xfce.org/thunar/ThunarUserManager.html  

    GObject
    ├── ThunarGroup
    ├── ThunarUser
    ╰── ThunarUserManager

    
    
* thunar-util
    
    https://developer.xfce.org/thunar/thunar-thunar-util.html  
    
#### Device Management

* ThunarDevice

    GObject
    ╰── ThunarDevice

* ThunarDeviceMonitor

    GObject
    ╰── ThunarDeviceMonitor

* thunar-notify
    
    https://developer.xfce.org/thunar/thunar-thunar-notify.html  
    
    Functions using ThunarDevice etc...



* ThunarFolder
    
    ```
    GObject
    ╰── ThunarFolder
    ```
    
* ThunarFileMonitor

    GObject
    ╰── ThunarFileMonitor


#### DnD

* thunar-dnd
    
    GdkDragAction 	thunar_dnd_ask ()
    gboolean 	thunar_dnd_perform ()


