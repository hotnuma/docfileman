**[ [Home](00-Home.html) | [Core](01-Core.html) | [Dialog](02-Dialog.html) | [Job](03-Job.html) | [Misc](05-Misc.html) | [Side](06-Side.html) | [View](07-View.html) | [Widget](08-Widget.html) | [Other](99-Other.html) ]**

## Dialog

---

* ThunarChooserDialog

    File Open / Save dialog box.
    
    ```
    ╰── GtkWindow
    ╰── GtkDialog
        ╰── ThunarAbstractDialog
            ╰── ThunarChooserDialog
    ```

    thunar/thunar-launcher.c:782:          thunar_show_chooser_dialog (launcher->widget, lp->data, TRUE);
    thunar/thunar-launcher.c:1244:    thunar_show_chooser_dialog (launcher->widget, launcher->files_to_process->data, TRUE);
    thunar/thunar-dbus-service.c:454:  thunar_show_chooser_dialog (screen, file, open);
    thunar/thunar-file.c:1830:      thunar_show_chooser_dialog (parent, file, TRUE);
    thunar/thunar-file.c:1841:      thunar_show_chooser_dialog (parent, file, TRUE);

* ThunarChooserModel

    ```
    ╰── GtkTreeStore
        ╰── ThunarChooserModel
    ```

* ThunarChooserButton

    https://developer.xfce.org/thunar/ThunarChooserButton.html  
    
    The "Open with" combo box in the properties dialog.  
    
    ```
    ╰── GtkComboBox
        ╰── ThunarChooserButton
    ```

    ```
    thunar-properties-dialog.c : thunar_properties_dialog_init
    
    dialog->openwith_chooser = thunar_chooser_button_new ();
    ```


