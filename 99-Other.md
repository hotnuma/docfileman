**[ [Home](00-Home.html) | [Core](01-Core.html) | [Dialog](02-Dialog.html) | [Job](03-Job.html) | [Misc](05-Misc.html) | [Side](06-Side.html) | [View](07-View.html) | [Widget](08-Widget.html) | [Other](99-Other.html) ]**

## Other

---

#### References

* Docs
    
    https://developer.xfce.org/thunar/index.html  
    https://wiki.xfce.org/thunar/dev/build_and_run  
    https://gitlab.xfce.org/xfce/thunar  
    https://docs.xfce.org/xfce/thunar/start  

* Build deps
    
    ```
    sudo apt install libnotify-dev libgudev-1.0-dev libexo-2-dev
    sudo apt install libxfconf-0-dev libxfce4util-dev libxfce4ui-2-dev libthunarx-3-dev
    ```



#### Biggest files

```
find . -type f -name "*.c" -printf "%s\t%p\n" | sort -nr | head -10

127510	./view/standard_view.c
102177	./core/th_file.c
95904	./menu/launcher.c
70707	./view/listmodel.c
70126	./side/treeview.c
68427	./window.c
60747	./side/treemodel.c
60213	./job/transfer_job.c
54371	./application.c
50846	./dialog/permbox.c
```



#### Notes

* selection change
    
    `standard_view_selection_changed`

* double clic detail view

    details_view_row_activated

        launcher_activate_selected_files (launcher, THUNAR_LAUNCHER_CHANGE_DIRECTORY, NULL);

#### Custom Actions

xfce_spawn_on_screen_with_child_watch : executes external program

match patterns : g_pattern_match_simple


