### Check if a string contains only numbers

```javascript
const isOnlyWholeNumbers = (str) => /^\d+$/.test(str)
```

This only takes into account whole numbers, but the following does :

```javascript
const isOnlyRealNumbers = (str) => /^\d+\.\d+$/.test(str)
```