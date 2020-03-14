# Advanced Screenshots with Firefox

Firefox already ships with a tool to generate screenshots of webpages you visit. However, the GUI tool is fairly limited in functionality.
To take advanced screenshots, e.g. with a high DPR, you can use the web console.

The following command will generate a full-page screenshot with a DPR of 2, instead of the standard DPR of 1.
```
:screenshot --dpr 2 --fullpage
```

More available commands:

* `--clipboard` Copies the screenshot to the clipboard
* `--delay 5` Waits the specified number seconds before taking the screenshot
* `--dpr 2` Uses the specified device-to-pixel ratio for the screenshot
* `--file` Saves the screenshot to a file, even if the --clipboard argument is specified
* `--filename screenshot.png` Saves the screenshot under the specified filename
* `--fullpage` Takes a screenshot of the full page, not just the currently visible area
* `--selector "#id"` Takes a screenshot of the element that matches the specified CSS query selector

_Source: [Dr. Link Check blog](https://www.drlinkcheck.com/blog/high-dpi-website-screenshot-firefox)_
