**[ [Home](00-Home.html) | [Core](01-Core.html) | [Dialog](02-Dialog.html) | [Job](03-Job.html) | [Misc](05-Misc.html) | [Side](06-Side.html) | [View](07-View.html) | [Widget](08-Widget.html) | [Other](99-Other.html) ]**

## Job

---

#### Files

```
    job/dcount_job.c
    + job/exo_job.c
    + job/io_jobs.c
    job/io_scan_directory.c
    + job/job.c
    job/job_utils.c
    job/simple_job.c
    job/transfer_job.c
```


#### ExoJob

* Description

    GObject used to wrap threaded/asynchronous operations in an object
    oriented way. It uses internally a GIOSchedulerJob.


#### ThunarJob

* Description

    An ExoJob used in dialogs and in file operations.


#### io_jobs

* Description

    Functions to execute IO jobs.

```
    io_list_directory
    io_make_directories
    io_create_files
    io_unlink_files
    io_move_files
    io_copy_files
    io_link_files
    io_trash_files
    io_restore_files
    io_rename_file
    io_change_group
    io_change_mode
```


