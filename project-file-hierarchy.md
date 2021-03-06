# Project file hierarchy

The directory structure of an android project.

<http://stackoverflow.com/questions/4761406/complete-list-of-all-android-resource-folders>

-   `AndroidManifest`: mandatory file with global configurations
-   `res`: resources. Both configuration strings like `values/strings.xml`, and media like images and audio. Documented at: <http://developer.android.com/guide/topics/resources/providing-resources.html>
    -   `drawable-<density>`: images to render.
        -   Densities are documented at: <http://developer.android.com/guide/practices/screens_support.html>
            - `ldpi` (low) ~120dpi
            - `mdpi` (medium) ~160dpi
            - `hdpi` (high) ~240dpi
            - `xhdpi` (extra-high) ~320dpi
            - `xxhdpi` (extra-extra-high) ~480dpi
            - `xxxhdpi` (extra-extra-extra-high) ~640dpi
            There is also:
            - `drawable-ldrtl-<density>`, which stands for "layout-direction-right-to-left", e.g. Arabic and Hebrew.
    - `values/strings.xml`: `<string name="app_name">MyActivity</string>`
-   `gen`: generated classes, e.g. `View` classes from `res/layout/mylayout.xml` files.
