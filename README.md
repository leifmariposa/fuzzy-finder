# Taz Fuzzy Finder package

Fork of the Fuzzy Finder package where <kbd>cmd-t</kbd> has been remapped to a new switch tab finder and the layout has been changed to only use one line.

To be used together with package taz-tab-switcher and taz-dark-ui/taz-light-ui theme.

Quickly find and open files using <kbd>cmd-t</kbd>.

  * <kbd>cmd-t</kbd> or <kbd>cmd-p</kbd> to open the file finder
  * <kbd>cmd-b</kbd> to open the list of open buffers
  * <kbd>cmd-shift-b</kbd> to open the list of Git modified and untracked files
  * <kbd>enter</kbd> defaults to opening the selected file without leaving the current pane
  * <kbd>shift-enter</kbd> defaults to switching to another pane if the file is already open there

Turning on the "Search All Panes" setting reverses the behavior of <kbd>enter</kbd> and <kbd>shift-enter</kbd> so <kbd>enter</kbd> opens the file in any pane and <kbd>shift-enter</kbd> creates a new tab in the current pane.

This package uses both the `core.ignoredNames` and `fuzzy-finder.ignoredNames` config settings to filter out files and folders that will not be shown. Both of those config settings are interpreted as arrays of [minimatch](https://github.com/isaacs/minimatch) glob patterns.

This package also will also not show Git ignored files when the `core.excludeVcsIgnoredPaths` is enabled.

![](https://f.cloud.github.com/assets/671378/2241456/100db6b8-9cd3-11e3-9b3a-569c6b50cc60.png)
