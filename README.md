dtct
====

Compare two (code) trees with or without a graphical diff.

### Notes

I suppose we've all written this one at least once, or get by typing complex shell commands. Maybe this is easier.

_dt_ compares two trees, indicating equality ('=') or difference ('DIFFERENT') on the console for each pair of files and displaying differing pairs in a graphical diff tool (controlled by variable _difftool_ in _dt_ and set by default to _xxdiff -D_). _dt_ tests and reports on the console differences in binary files, but tries to avoid opening them in _difftool_. It also gives a final report of files that were present in only one of the two trees.

_ct_ calls _dt_ with the optional _nodiff_ argument to disable graphical diffs.

### Requirements

_ksh_ and standard GNU shell utilities like _file_, _sed_, _uniq_, etc. If you don't like _ksh_, _dt_ and _ct_ could be trivially rewritten in _bash_.

### License

The contents of this repository are released under the [Apache 2.0](http://www.apache.org/licenses/LICENSE-2.0) license. See the LICENSE file for details.
