# en_001
This repository contains a glibc locale definition file for "en_001", or international English – "001" being the Unicode name for [The World](https://icu4c-demos.unicode.org/icu-bin/locexp?d_=en&_=en_001).

 * All text is, unsurprisingly, in English.
 * Dates follow [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601).
 * The week begins on Monday.
 * The default paper size is A4.
 * Measurements are in metric.
 * Numbers use a dot as decimal separator.
 * Collation uses the base [ISO 14651](https://en.wikipedia.org/wiki/ISO/IEC_14651) algorithm, "iso14651_t1_common".
 * The currency symbol is the [international currency sign ¤](https://en.wikipedia.org/wiki/Currency_sign_(typography)).
 * The telephone prefix is [882](https://en.wikipedia.org/wiki/International_Networks_(country_code)).

## Installation
This process works for Gentoo. YMMV for other distributions.
1. Stick the "en_001" file into `/usr/share/i18n/locales/`.
2. Run `localedef -i en_001 -f UTF-8 en_001.UTF8`.
3. Edit `/etc/locale.gen` and add `en_001.UTF8 UTF-8` to it.
4. Run `locale-gen`.
5. Done! The locale can now be used.
