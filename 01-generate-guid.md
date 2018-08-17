---
tags: javascript,identifier,key
---

```javascript
function guid() {
  function s4() {
    return Math.floor((1 + Math.random()) * 0x10000)
      .toString(16)
      .substring(1);
  }
  return s4() + s4() + '-' + s4() + '-' + s4() + '-' + s4() + '-' + s4() + s4() + s4();
}

// => "0153a717-3ba2-b1ac-67f1-49db6551a28d"
```
