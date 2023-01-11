# ff14-fish-tracker-app-data

A place to store data files necessary for the backend for the Discord bot Fisher's Intuition.  Update to this repo are deployed automatically.

Two data files from CarbunclePlushy's tracker are utilized with the following adjustments:

## https://github.com/icykoneko/ff14-fish-tracker-app/blob/master/js/app/fish_info_data.js
Replace first line:
```js
const FISH_INFO = [
```
with the following two lines:
```js
FISH_INFO = {
  FISH_INFO_DATA: [
```
and replace final line:
```js
 ];
```
with three lines:
```js
 ]
}
module.exports = FISH_INFO
```

## https://github.com/icykoneko/ff14-fish-tracker-app/blob/master/js/app/data.js
Replace first line:
```js
const DATA = {
```
with the following line:
```js
DATA = {
```
And add after final line:
```js
module.exports = DATA
```

## Submitting an update with data used with [CarbyUtils.setFishConditions()](https://github.com/icykoneko/ff14-fish-tracker-app/wiki/Tips-for-New-Fish-Conditions-Research)

1. Use CarbyUtils as normal, to update fish windows
2. At the same console, type `DATA` and on the object that comes back, right click -> Copy object 
3. Update `data.js` in this repo by replacing the object assigned to DATA with the copied object
4. Commit the changes and submit a pull request to this repo.
