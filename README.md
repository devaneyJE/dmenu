## devaneyJE: dmenu configuration
This repo contains my personal configuration for `dmenu`, including patches and other modifications to the source for the original project found at [suckless.org](https://tools.suckless.org/dmenu/).

### Patches:
Diffs from the patch versions used in this utility are included in the [patches](../tree/main/patches) directory. The following patches are currently in use:

- [border](https://tools.suckless.org/dmenu/patches/border/): Provides border around dmenu matching primary selection color.
- [caseinsensitive](https://tools.suckless.org/dmenu/patches/case-insensitive/): Case insensitivity becomes default behavior, replacing insensitive flag with `-s` flag for enabling sensitive matching.
- [fuzzymatch](https://tools.suckless.org/dmenu/patches/fuzzymatch/): Matches non-consecutive portions of provided strings in search.
- [grid](https://tools.suckless.org/dmenu/patches/grid/): Provides option to display menu in multiple rows and columns.
- [gridnav](https://tools.suckless.org/dmenu/patches/gridnav/): Provides left/right navigation support in grid layout.
- [numbers](https://tools.suckless.org/dmenu/patches/numbers/): Displays number of matches and total items in dmenu.

### Colors:
```C
static const char colors*[SchemeLast][2] = {
    [SchemeNorm] = { "#bbbbbb", "#222222" },
    [SchemeSel] = { "#eeeeee", "#415a78" },
    [SchemeOut] = { "#000000", "#00ffff" },
};
```

### Contributions:
Credit for the primary tool is listed in the original, included [license](/LICENSE). Authors of the various scripts in the [dmscripts](/dmscripts) directory are credited within each file. Scripts included may reflect either code of original author(s), or modifications I made to the script.