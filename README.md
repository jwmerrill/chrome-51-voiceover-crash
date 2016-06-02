# Chrome 51 VoiceOver crash demonstration

Demonstrates a font-related crash bug in Chrome 51 when using OS X VoiceOver. To observe the crash, open `crashes.html` in Chrome 51 on OS X, activate VoiceOver (cmd-F5), and focus the `y=x` input box.

`works.html` is a very similar setup that does not cause a crash. The only difference is that it uses a different set of font files for the Symbola font: `works.html` loads Symbola from `lib/font/Symbola.[woff|ttf]`, and `crashes.html` loads a subsetted version of Symbola from `lib/font/Symbola-basic.[woff|ttf]`.

This demonstration uses the open source math typesetting library [MathQuill](http://mathquill.com/), and was first observed in the [Desmos online graphing calculator](https://www.desmos.com/calculator), which currently crashes in Chrome 51 with voiceover activated.
