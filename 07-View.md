**[ [Home](00-Home.html) | [Core](01-Core.html) | [Dialog](02-Dialog.html) | [Job](03-Job.html) | [Misc](05-Misc.html) | [Side](06-Side.html) | [View](07-View.html) | [Widget](08-Widget.html) | [Other](99-Other.html) ]**

## View

---

* ./thunar/thunar-details-view.c
    
    206: thunar_details_view_init
    
    tree_view = exo_tree_view_new ();

    click in the detail view
    
    646: thunar_details_view_button_press_event

    ```
    thunar_details_view_init:
    
    /* configure the tree selection */
    selection = gtk_tree_view_get_selection (GTK_TREE_VIEW (tree_view));
    gtk_tree_selection_set_mode (selection, GTK_SELECTION_MULTIPLE);
    g_signal_connect_swapped (G_OBJECT (selection), "changed",
                            G_CALLBACK (thunar_standard_view_selection_changed), details_view);
    ```



    
* ./thunar/thunar_list_model.c
    
    
