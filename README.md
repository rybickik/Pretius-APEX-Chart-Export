# Pretius-APEX-Chart-Export
Pretius APEX Chart Export is a simple plugin that enables users to export Oracle APEX charts to PNG file just with two clicks.

The plugin uses SaveSvgAsPng (https://github.com/exupero/saveSvgAsPng) and jQuery Context Menu (https://github.com/swisnl/jQuery-contextMenu) libraries.

## Preview
![](/pretius_apex_chart_export_preview.gif?raw=true)

## Table of Contents
- [License](#license)
- [Demo Application](#demo-application)
- [Roadmap](#roadmap)
- [Install](#install)
- [Usage guide](#usage-guide)
- [Changelog](#changelog)
  - [1.0](#10)
- [About Author](#about-author)
- [About Pretius](#about-pretius)
- [Support](#support)
  - [Free support](#free-support)
  - [Paid support](#paid-support)

## License
MIT

## Demo Application
[Pretius APEX Chart Export demo application](https://apex.oracle.com/pls/apex/krybicki/r/pretius-apex-chart-export)

## Roadmap
* [ ] Support for Internet Explorer browser
* [ ] Possibility to customize SaveSvgAsPng library options
* [ ] Possibility to export charts using APEX buttons
* [ ] Support for other Oracle JET components (like Gantts, Gauges, Thematic Maps etc.)

## Install
To successfully install/update the plugin follow those steps:
1. Install the plugin file `dynamic_action_plugin_com_pretius_apex_chart_export.sql` using Oracle APEX plugin import wizard

## Usage guide
1. Set `Static ID` for chart regions
1. Create new dynamic action
  * Set `Event` to `Page Load`
  * Go to `True actions`
1. Create new `True action`
1. Change Action to `Pretius APEX Chart Export [Plug-In]`
1. Set `Fire On Page Load` to `Yes` (if it's not set)
1. Save, run the page and test chart export by right clicking on the chart and the 'Save as PNG' menu item

Please be aware that exported file name depends on chart region static ID. 

## Changelog

### 1.0
Initial release

## About Author
Author            | Github                                       | Twitter                                       | E-mail
------------------|----------------------------------------------|-----------------------------------------------|----------------------------------------------------
Kamil Rybicki | [@rybickik](https://github.com/rybickik) | [@rybicki_k](https://twitter.com/rybicki_k) | krybicki@pretius.com

## About Pretius
Pretius Sp. z o.o. Sp. K.

Address | Website | E-mail
--------|---------|-------
Żwirki i Wigury 16a Warsaw 02-092, Poland | [https://pretius.com/](https://pretius.com/) | [office@pretius.com](mailto:office@pretius.com)

## Support
Our plugins are free to use but in some cases you might need to contact us. We are willing to assist you but in certain circumstances you will be charged for our time spent on helping you. Please keep in mind we do our best to keep documentation up to date and we won't answer question for which there is explaination in documentation (at github and as help text in application builder).

All request (bug fix / change request) should be posted in Issues Tab at github repository.

### Free support
We do support the plugin in certain cases such as bug fixing and change request. If you have faced issue that might be bug please check Issues tab in github repository. In case you won't be able to find related issue please raise the issue following these rules:

* issue should contain login credentials to application at apex.oracle.com where issue is reproduced
* issue should contain steps to reproduce the issue in demo application
* issue should contain description about it's nature

### Paid support
In case you are not able to implement the plugin or you are willing to have custom implementation based on the plugin attributes (ie. custom JavaScript callbacks) we are willing to help you. Please send inquiry to apex[at]pretius.com with description what you want us to help you with. We will contact you as soon as possible with pricing and possible dates.
