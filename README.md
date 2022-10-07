# ZapMe Backend UnitTest DataSet

This repository contains the dataset used for the unit tests of the ZapMe backend.

Note: **These files are NOT used for the ZapMe backend itself, but ONLY for the unit tests to verify the correct behavior of the backend.**

Currently, the dataset contains the following data:

## Text

This folder contains text that is used to verify the blacklist filter for Usernames, Displaynames, GroupNames, Statuses, etc...

- `locales.json` contains locales that is fed to [Bogus](https://github.com/bchavez/Bogus) to generate random text for the unit tests.
- `WhiteList/` folder that contains charsets and text that should all pass the blacklist filter.
   - `CharSets/` folder that contains files categorized by language or usage, these files contain newline separated characters that should all pass the blacklist filter.
   - `Text/` folder that contains random text (Lorem Ipsum, Pull Requests, etc...). These files should all pass the blacklist filter.
- `BlackList/` folder that contains charsets and text that should all fail the blacklist filter.
   - `CharSets/` folder that contains files categorized by language or usage, these files contain newline separated characters that should all fail the blacklist filter.
   - `Text/` folder that contains random text (Lorem Ipsum, Pull Requests, etc...). These files should all fail the blacklist filter.

## Contributing

Feel free to contribute to this repository by adding more text to the `WhiteList/` and `BlackList/` folders.