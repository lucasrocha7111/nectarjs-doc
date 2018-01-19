# Incluir C

NectarJS permite que você inclua C em seus módulos. Um simples exemplo :

myModule/c/file.c :

```c
var simpleInt()
{
  printf("In C Function\n");
  return __N_Create_Int(42);
}
```

myModule/index.js :

```javascript
//!_c_include "c/file.c"

console.log(simpleInt());

```
