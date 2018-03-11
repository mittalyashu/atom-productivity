# Walkthought

### Side Bar

Sublime’s side bar contains a browsable list of files and folders. You can expand nested folders to show their contents, open the files for editing, or preview their contents.

While the side bar provides convenient access to open files and folders, it also imposes some surprising limitations in its out-of-the-box configuration. You can’t can’t drag and drop files or folders to rearrange them, and the right-click menus provide only basic file commands.

### Toggling the Side Bar

When you first install Sublime, the side bar should be enabled by default. You can quickly toggle it off if you’d like to devote more screen real estate to your code and reenable it when you need to browse for another file.

To toggle the side bar:

* Click View \| Side Bar \| Show Side Bar or View \| Side Bar \| Hide Side Bar.
  Or press Command+K,Command+B on Mac OS X or Ctrl+K,Ctrl+B on Windows and Linux.

### Previewing Files

Sublime’s preview feature is one of those subtle touches that can make a big difference in your day-to-day work. I frequently find myself hunting through multiple files, looking for a particular piece of code. In most editors, each file I examine opens in a new tab, and before long I have two dozen tabs open.

> **\[info\] Preview tabs**
>
> In Sublime Text 3, single-clicking a file opens the preview in a special temporary tab. You can identify this tab by the italicized file name in the tab’s title. The preview tab is reused  
> when you single-click another file.
>
> It’s an improvement over the old model where the preview took over the active tab because it allows you to peek at files while still referring to the files you’re actively working on.
>
> If you start editing the file, Sublime promotes the preview tab to a regular tab.

### Opening Folders

The Folders section of the side bar shows any folders you’ve opened in Sublime, as well as the files they contain.

To add a folder to the side bar:
* Drag the folder from your file explorer into the Sublime side bar. Or, on Mac OS X, drag the folder into the Sublime icon on the dock.

You can tell Sublime not to show selected folders or file types in the side bar. This is convenient for hiding files that Sublime can’t edit, such as .png graphics, or for excluding the compiled outputs of platforms such as CoffeeScript or SASS. To customize Sublime’s file exclusions, see the `folder_exclude_patterns`,  `file_exclude_patterns` and `binary_-file_patterns` settings in the `Preferences.sublime-settings` file. You can override the defaults in your user-specific settings, and you can also customize them on a per-project level.

