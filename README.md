dtct
====

Compare two (code) trees with or without a graphical diff.

### Notes

I suppose we've all written this one at least once, or get by typing complex shell commands. Maybe this is easier.

`dt` compares two trees, indicating equality ('=') or difference ('DIFFERENT') for each files on the console, and displaying differing pairs in a graphical diff tool (controlled by variable _difftool_ in `dt` -- set by default to _xxdiff -D_). `dt` tests and reports on the console differences in binary files, but tries to avoid opening them in _difftool_. It also gives a final report about files that were present in only one of the trees.

`ct` calls `dt` with the optional _nodiff_ final argument to avoid any graphical diffs.

### License

The contents of this repository are released under the [Apache 2.0](http://www.apache.org/licenses/LICENSE-2.0) license. See the LICENSE file for details.
