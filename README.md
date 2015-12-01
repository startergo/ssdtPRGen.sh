ssdtPRGen.sh
============

You can download the latest Beta of ssdtPRGen.sh by entering the following command in a terminal window:

``` sh
curl -o ~/ssdtPRGen.sh https://raw.githubusercontent.com/Piker-Alpha/ssdtPRGen.sh/Beta/ssdtPRGen.sh
```

This will download ssdtPRGen.sh to your home directory (~) and the next step is to change the permissions of the file (add +x) so that it can be run.
 
``` sh
chmod +x ~/ssdtPRGen.sh
```

Note: ssdtPRGen.sh v15.1 and greater require a working Internet connection so that it can download configuration data and command line tools. You can also download a complete zip archive by entering the following commands in a terminal window:

``` sh
curl -o ~/Library/ssdtPRGen.zip https://codeload.github.com/Piker-Alpha/ssdtPRGen.sh/zip/Beta
unzip -qu ~/Library/ssdtPRGen.zip -d ~/Library/
mv ~/Library/ssdtPRGen.sh-Beta ~/Library/ssdtPRGen
rm ~/Library/ssdtPRGen.zip
```


Help Information
----------------

``` sh
$ ~/ssdtPRGen.sh -h

Usage: ./ssdtPRGen.sh [-abcdfhlmptwx]
       -acpi Processor name (example: CPU0, C000)
       -bclk frequency (base clock frequency)
       -board-id (example: Mac-F60DEB81FF30ACF6)
       -cpu type [0/1/2/3]
          0 = Sandy Bridge
          1 = Ivy Bridge
          2 = Haswell
          3 = Broadwell
       -debug output [0/1/3]
          0 = no debug injection/debug output
          1 = inject debug statements in: ssdt.dsl
          2 = show debug output
          3 = both
       -frequency (clock frequency)
       -help info (this)
       -lfmode, lowest idle frequency
       -logical processors [2-128]
       -model (example: MacPro6,1)
       -open the previously generated SSDT
       -processor model (example: 'E3-1285L v3')
       -show supported board-id and model combinations:
           Haswell
           Ivy Bridge
           Sandy Bridge
       -turbo maximum (turbo) frequency:
          6300 for Sandy Bridge and Ivy Bridge
          8000 for Haswell and Broadwell
       -tdp [11.5 - 150]
       -workarounds for Ivy Bridge [0/1/2/3]
          0 = no workarounds
          1 = inject extra (turbo) P-State at the top with maximum (turbo) frequency + 1 MHz
          2 = inject extra P-States at the bottom
          3 = both
       -xcpm mode [0/1]
          0 = XCPM mode disabled
          1 = XCPM mode enabled
```

Bugs
----

All possible bugs (so called 'issues') should be filed at:

https://github.com/Piker-Alpha/ssdtPRGen.sh/issues

Please do **not** use my blog for this. Thank you!

