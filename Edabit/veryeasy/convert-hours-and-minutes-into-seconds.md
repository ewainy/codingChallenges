# Convert Hours and Minutes into Seconds

Write a function that takes two integers `(hours, minutes)`, converts them to seconds, and adds them.

## Examples
convert(1, 3) ➞ 3780

convert(2, 0) ➞ 7200

convert(0, 0) ➞ 0

```js
function convert(hours, minutes) {
	return (hours * 60 * 60) + (minutes * 60)
}
```
