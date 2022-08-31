# ff14-fish-tracker-app-data

A place to store data files necessary for the Discord bot backend derived from https://github.com/icykoneko/ff14-fish-tracker-app

Two data files from above repo are utilized with the following adjustments:

## https://github.com/icykoneko/ff14-fish-tracker-app/blob/master/js/app/fish_info_data.js
Replace first line:
```js
const FISH_INFO = [
```
with the following two lines:
```js
module.exports = FISH_INFO = {
  FISH_INFO_DATA: [
```
and replace final line:
```js
 ];
```
with two lines:
```js
 ]
}
```

## https://github.com/icykoneko/ff14-fish-tracker-app/blob/master/js/app/data.js
Replace first line:
```js
const DATA = {
```
with the following line:
```js
module.exports = DATA = {
```
