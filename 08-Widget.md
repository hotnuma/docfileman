**[ [Home](00-Home.html) | [Core](01-Core.html) | [Dialog](02-Dialog.html) | [Job](03-Job.html) | [Misc](05-Misc.html) | [Side](06-Side.html) | [View](07-View.html) | [Widget](08-Widget.html) | [Other](99-Other.html) ]**

## Widget

---

#### Entry

* ThunarLocationEntry

    https://developer.xfce.org/thunar/ThunarLocationEntry.html  

    ```
    ╰── GtkWidget
        ╰── GtkContainer
            ╰── GtkHBox
                ╰── ThunarLocationEntry
    ```


* ThunarPathEntry

    ╰── GtkWidget
        ╰── GtkEntry
            ╰── ThunarPathEntry

    `thunar/thunar-location-entry.c:190:  location_entry->path_entry = thunar_path_entry_new ();`


#### Image/Icon

* ThunarImage
    
    https://developer.xfce.org/thunar/ThunarImage.html  
    
    ```
    ╰── GtkWidget
        ╰── GtkMisc
            ╰── GtkImage
                ╰── ThunarImage
    ```
    
    Contains a ThunarFileMonitor and a ThunarFile.
    
    The icon used in ThunarPropertiesDialog :
    
    ```
    thunar/thunar-properties-dialog.c:285:  dialog->icon_image = thunar_image_new ();
    ```


