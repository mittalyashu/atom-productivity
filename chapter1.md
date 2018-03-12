# Walkthought

### Side Bar

Atom side bar contains a browsable list of files and folders. You can expand nested folders to show their contents, open the files for editing, or preview their contents.

While the side bar provides convenient access to open files and folders, it also imposes some surprising limitations in its out-of-the-box configuration. You can drag and drop files or folders to rearrange them, and the right-click menus provide file commands.

### Toggling the Side Bar

When you first install Atom, the side bar should be disabled by default. You can quickly toggle it on if you’d like to devote more screen real estate to your code and re-enable it when you need to browse for another file.

To toggle the side bar:

* Click **View \| Side Bar \| Show Side Bar** or **View \| Side Bar \| Hide Side Bar**.
  Or press **Command+\**, on Mac OS X or **Ctrl+\** on Windows and Linux.

### Previewing Files

Atom's preview feature is one of those subtle touches that can make a big difference in your day-to-day work. I frequently find myself hunting through multiple files, looking for a particular piece of code. In most editors, each file I examine opens in a new tab, and before long I have two dozen tabs open.

> **\[info\] Preview tabs**
>
> In Atom, single-clicking a file opens the preview in a special temporary tab. You can identify this tab by the italicized file name in the tab’s title. The preview tab is reused when you single-click another file.
>
> It’s an improvement over the old model where the preview took over the active tab because it allows you to peek at files while still referring to the files you’re actively working on.
>
> If you start editing the file, Atom promotes the preview tab to a regular tab.

### Opening Folders

The Folders section of the side bar shows any folders you’ve opened in Atom, as well as the files they contain.

To add a folder to the side bar:

* Drag the folder from your file explorer into the Atom side bar. Or, on Mac OS X, drag the folder into the Atom icon on the dock.

> **\[info\] Preview tabs**
>
> You can tell Atom not to show selected folders or file types in the side bar. This is convenient for hiding files that Atom can’t edit, such as .png graphics, or for excluding the compiled outputs of platforms such as CoffeeScript or SASS. To customize Atom’s file exclusions, see the `folder_exclude_patterns`,  `file_exclude_patterns` and `binary_-file_patterns` settings in the `Preferences.atom-settings` file. You can override the defaults in your user-specific settings, and you can also customize them on a per-project level.

### Toggling the Open Files Section

By default, the side bar is divided into two sections, **Folders** and **Open Files.**

The **Open Files** section shows dots on files that have been modified and close icons on unmodified files.

You can hide the **Open Files** section if you’d prefer, since it doesn’t provide much information that you can’t already glean from your list of tabs.

To toggle the **Open Files** section:

* **Click View | Side Bar | Hide Open Files** or **View | Side Bar | Show Open Files.**

### Menus

While the Sublime Side Bar is helpful for basic navigation and for visualizing your project’s structure, it offers only a barebones set of commands for working with the files and folders that make up your project.

The Side Bar has three different right-click menus, and they’re all pretty bare bones.

Right-clicking a file in the Open Files section reveals only a Close option, which closes the file’s tab.

In the Folders section, right-clicking on a folder brings up a menu with a few basic options: New File, Rename…, New Folder, Delete Folder and Find in Folder. New File, New Folder and Rename… open an input panel at the bottom of the screen that allows you to enter the desired file or folder name. The Find in Folder option opens a Find panel and populates the folder name into the Where…
field.

> **\[warning\] Deleting a folder with open files**
>
> When you use the Delete Folder command, Atom doesn’t close tabs for files that were contained in the deleted folder. The tabs remain open as if nothing happened, but you’ll get an error message if you make changes and attempt to save the file.


Right-clicking a file in the Folders section brings up just three options: Rename, Delete File and Open Containing Folder… Rename opens an input panel where you can type the new file name. Selecting the Delete option removes the file and closes any open tabs associated with it.

Version Difference!

In Sublime Text 2, deleting a file from the Side Bar removes it from the file system but leaves it open in a tab, changes the tab to unsaved. Easy to accidentally restore the file by

saving the tab.

The Open Containing Folder command opens your system file manager to the parent folder of the
selected file.

Rearranging files

Since the Side Bar doesn’t allow you to drag and drop files to reorganize them, using
Open Containing Folder to and then shuffling files in your file manager is often the best
workaround.
