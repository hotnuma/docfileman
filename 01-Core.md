**[ [Home](00-Home.html) | [Core](01-Core.html) | [Dialog](02-Dialog.html) | [Job](03-Job.html) | [Misc](05-Misc.html) | [Side](06-Side.html) | [View](07-View.html) | [Widget](08-Widget.html) | [Other](99-Other.html) ]**

## Core

---

#### Files

```
    + core/clipboard.c
    + core/devmonitor.c
    + core/dnd.c
    + core/fileinfo.c
    + core/filemonitor.c
    + core/th_device.c
    + core/th_file.c
    + core/th_folder.c
    + core/user.c
```


#### User

* Description

    This module provides three objects, a global UserManager,
    a ThunarGroup and ThunarUser. The PermissionBox uses it.


#### ClipboardManager

* Description

    A GObject to handle cut, copy, paste clipboard operations on files,
    it uses GtkClipboard internally.


#### DnD

* Description

    dnd_ask
    
    dnd_perform


#### ThunarDevice

* Description

    A GObject which uses a GVolume, GMount or GDrive to handle devices.


#### DeviceMonitor

* Description

    A global GObject to handle device events, it uses GVolumeMonitor
    internally. ThunarDevice, TreeModel and Window use it.


#### ThunarFile

* Description

    A GObject to handle file informations. The th_file_info_reload function
    loads these informations.

* File sorting

    The th_file_compare_by_name function calls g_utf8_collate_key_for_filename
    to compare file names.


#### FileInfo

* Description

    A GTypeInterface to handle file infos using GFile and GFileInfo.


#### ThunarFolder

* Description

    A GObject to handle folders which uses a ThunarJob, ThunarFile,
    FileMonitor and GFileMonitor.


#### FileMonitor

* Description

    A global GObject to handle file events.


