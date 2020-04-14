# inkdrop-insert-date

A plugin for [Inkdrop](https://www.inkdrop.app/) that allows you to quickly insert the current date and time into your notes. Uses [Moment.js](https://momentjs.com/) for formatting and localization.
It was originally created by [@sambrezo](https://github.com/sambrezo/inkdrop-insert-date).

## Install

```sh
ipm install insert-date
```

## Usage

Just right-click in the editor to open the context menu and select `Insert date`.

Alternatively you can add a keybinding to your `keymap.cson` file like so:

```js
{
  "body": {
    "ctrl-alt-d": "insert-date:run"
  }
}
```

## Settings

Please refer to Moment.js for all available [displaying options](https://momentjs.com/docs/#/displaying/) and [supported locales](https://github.com/moment/moment/tree/2.22.1/locale).

### Format

Here are some common options you can choose from:

- `MMMM Do YYYY, h:mm:ss a`: April 22nd 2016, 5:14:58 am
- `LT`: 5:14 AM
- `LTS`: 5:14:58 AM
- `L`: 04/22/2016
- `l`: 4/22/2016
- `LL`: April 22, 2016
- `ll`: Apr 22, 2016
- `LLL`: April 22, 2016 5:14 AM
- `lll`: Apr 22, 2016 5:14 AM
- **`LLLL`: Friday, April 22, 2016 5:14 AM (default)**
- `llll`: Fri, Apr 22, 2016 5:14 AM

### Locale

- **`en`: Friday, April 22, 2016 5:14 AM (default)**
- `ja`: 2016 年 4 月 22 日 金曜日 05:14
- `de`: Freitag, 22. April 2016 05:14
- `fr`: mardi 14 avril 2020 16:34
