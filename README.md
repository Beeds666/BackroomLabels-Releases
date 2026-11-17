# Backroom Labels — downloads

Prints shelf tags, sale signs and other labels from AEPOS, using the store's AzureLabel templates. Part of Backroom Suite.

## Install

The easiest way is Backroom Suite: **Apps → Backroom Labels → Install**. To install it by hand, download
`BackroomLabelsSetup-x.y.z.exe` from the newest release on the **Releases** page and run it. It needs 64-bit
Windows 10 or 11.

The app updates itself (**Check for updates** at the bottom of its window). PCs on Backroom Suite's test channel also
get test versions.

## Before the first print

1. In Backroom Suite, add the store and run **Set up store → Create or update views**. That creates the
   `BRS_AzureLabel` and `BRS_AzureLabelChanges` views this app reads. It only reads; it never changes AEPOS.
2. Open Backroom Labels. The standard templates (Yellow Corner, Green Corner, RTI, sale signs…) are added on its
   first run. **Import AzureLabel templates…** brings in your own `.altz` files.
3. Pick the printer, then **Line up printer…** → print the test page on plain paper, hold it over a label sheet,
   and enter how far off it is. It's kept for that printer.

## Where things are kept

- Templates: `Documents\Backroom Suite\Labels`
- Settings: `%LocalAppData%\BackroomLabels\prefs.json`
- Error log: `%LocalAppData%\BackroomLabels\error.log`

Uninstalling leaves templates and settings in place.
