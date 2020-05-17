# Extras for DutyMan

This repo hosts some extras to support users of [DutyMan](https://dutyman.biz/)
the duty management system.

The first to be implemented is:
* CSS style sheets for clearer embedding

## Installation

You don't need to install anything to use the default CSS stylesheets from
jsDelivr.

If you want to extend these with a style of your own, copy the relevant file
from `src/css`, adapt it and host it on your own web site.

## Usage

Set the `css` option in the DutyMan query string to point to your own file or one of ours served from the jsDelivr CDN.
```html
<iframe src="https://dutyman.biz/dmembed.aspx?id=M0000000&amp;css=https://cdn.jsdelivr.net/gh/pbinuk/dutyman/src/css/embed.css"
></iframe>
```

There are 12 files with different combinations of options as below (plus an
'all options' file which doesn't look great and is just for development).

### Options

Option | Description
-------|------------
`nolast` | Hide the last row because it is usually "...and more" - use with care.
`nolink` | Hide "All events and duties" link to Dutyman.
`center-date` | Centre the date - looks best in Modes 1 and 2.
`bold-event` | Highlight the dates and event names - looks best in Mode 3. 

file | Simple format | No last row | No link | Bold event| Centre date |
-------------|-------|---|---|---|---|
`embed`                          | ✓ |   |   |   |
`embed-bold-event`               | ✓ |   |   | ✓ |
`embed-center-date`              | ✓ |   |   |   | ✓
`embed-nolast`                   | ✓ | ✓ |   |   |
`embed-nolast-bold-event`        | ✓ | ✓ |   | ✓ |
`embed-nolast-center-date`       | ✓ | ✓ |   |   | ✓
`embed-nolink`                   | ✓ |   | ✓ |   |
`embed-nolink-bold-event`        | ✓ |   | ✓ | ✓ |
`embed-nolink-center-date`       | ✓ |   | ✓ |   | ✓
`embed-nolast-nolink`            | ✓ | ✓ | ✓ |   |
`embed-nolast-nolink-bold-event` | ✓ | ✓ | ✓ | ✓ |
`embed-nolast-nolink-center-date`| ✓ | ✓ | ✓ |   | ✓
`embed-all`                      | ✓ | ✓ | ✓ | ✓ | ✓
