**[ [Home](00-Home.html) | [Core](01-Core.html) | [Dialog](02-Dialog.html) | [Job](03-Job.html) | [Misc](05-Misc.html) | [Side](06-Side.html) | [View](07-View.html) | [Widget](08-Widget.html) | [Other](99-Other.html) ]**

## Fileman

---

#### Main

* Description
    
    The main function sets the application name, initializes libnotify and
    runs the application.



#### Application
    
* Description

    Application object is a GtkApplication, it contains functions to
    execute file operations.
    
    ```
    application_process_filenames
    application_mkdir
    application_creat
    application_copy_into
    application_link_into
    application_move_into
    application_unlink_files
    application_trash
    application_restore_files
    application_empty_trash
    ```
    
    For example, LAUNCHER_ACTION_CREATE_FOLDER menu item calls _launcher_action_create_folder
    then calls application_mkdir.
    


#### Popup Menu

* Description

    Popup menus are created from the TreeView and StandardView
    using g_object_new and appmenu_add_sections. First, the Launcher
    informations are filled, then the popup is created, then selecting
    an item will call a launcher function on the corresponding Launcher
    object.

* TreeView
    
    The menu is created from the widget's popup handler which calls the
    treeview_popup_menu function and then _treeview_context_menu.
    
* StandardView

    The widget creates its popup in response to a button-release-event signal,
    it calls the _standard_view_button_release_event function and then it calls
    standard_view_context_menu.



#### Launcher

* ThunarLauncher
    
    ThunarActionManager

    GObject
    


#### Window

* Description

    GtkWindow
    
    thunar_window_init
    
    ```
    GtkWindow window
    
        GtkGrid grid
            ___________________________________________________
            GtkToolbar toolbar
                GtkToolItem tool_item
                    LocationBar location_bar (GtkBox)
                        ThunarPathEntry (GtkEntry)
            ___________________________________________________
            GtkPaned paned (horizontal)
            pane1
                window_install_sidepane
                ThunarSidePane sidepane
            pane2
                GtkGrid view_box
                    GtkNotebook notebook
                    GtkStatusbar statusbar
            ___________________________________________________
    ```


