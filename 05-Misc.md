**[ [Home](00-Home.html) | [Core](01-Core.html) | [Dialog](02-Dialog.html) | [Job](03-Job.html) | [Misc](05-Misc.html) | [Side](06-Side.html) | [View](07-View.html) | [Widget](08-Widget.html) | [Other](99-Other.html) ]**

## Misc

---

* thunar-enum-types
    
    https://developer.xfce.org/thunar/thunar-thunar-enum-types.html  

    GEnum
    ├── ThunarColumn
    ├── ThunarDateStyle
    ├── ThunarFolderItemCount
    ├── ThunarIconSize
    ├── ThunarImagePreviewMode
    ├── ThunarJobOperationKind
    ├── ThunarOperationLogMode
    ├── ThunarParallelCopyMode
    ├── ThunarRenamerMode
    ├── ThunarThumbnailMode
    ├── ThunarThumbnailSize
    ├── ThunarUsePartialMode
    ├── ThunarVerifyFileMode
    ╰── ThunarZoomLevel
    GFlags
    ├── ThunarFileMode
    ╰── ThunarJobResponse




#### Interfaces
    
    ```
    $ cgrep GTypeInterface
    view/thunar-view.h:38:    GTypeInterface __parent__;
    side/thunar-side-pane.h:36:    GTypeInterface __parent__;
    misc/thunar-component.h:36:    GTypeInterface __parent__;
    misc/thunar-browser.h:58:    GTypeInterface __parent__;
    misc/thunar-navigator.h:36:    GTypeInterface __parent__;
    ```

* ThunarHistory

    https://developer.xfce.org/thunar/ThunarHistory.html  
    
    GObject
    ╰── ThunarHistory

* ThunarNavigator

    GInterface
    ╰── ThunarNavigator


* ThunarComponent

    GInterface
    ╰── ThunarComponent



* ThunarBrowser
    
    https://developer.xfce.org/thunar/ThunarBrowser.html  
    
    ```
    GInterface
    ╰── ThunarBrowser
    ```
    Resolves files to open.
    
    ```
    thunar-application.c:1573:  thunar_browser_poke_file (THUNAR_BROWSER (application), file, screen,
    thunar-window.c:3879:      thunar_browser_poke_location (THUNAR_BROWSER (window), current_directory, THUNAR_WINDOW (window),
    widget/thunar-location-entry.c:414:      thunar_browser_poke_file (THUNAR_BROWSER (location_entry), file, path_entry,
    core/thunar-launcher.c:929:       thunar_browser_poke_device (THUNAR_BROWSER (launcher), launcher->device_to_process,
    core/thunar-launcher.c:937:      thunar_browser_poke_file (THUNAR_BROWSER (launcher), poke_data->files_to_poke->data,
    core/thunar-launcher.c:1110:      thunar_browser_poke_file (browser, poke_data->files_to_poke->data,
    ```


