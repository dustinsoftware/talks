## Ember Octane: Build Tooling Changes

---

![](01.png)

---

## Improvement: Importing third party modules

---

## Before: Broccoli and ember-addons

---

https://github.com/mike-north/ember-lodash

https://simplabs.com/blog/2017/02/13/npm-libs-in-ember-cli.html

---

## After: ember-auto-import

https://github.com/ef4/ember-auto-import

---

Some advantages: 

* Defer loading large libraries until they are needed
* Remove large wrapper libraries

---

Before: 

![](https://user-images.githubusercontent.com/942358/54138487-f4864700-43f5-11e9-843a-0b5775f54b34.png)

After: 

![](https://user-images.githubusercontent.com/942358/54138511-fe0faf00-43f5-11e9-8279-dbda72f76ee9.png)

---

### Improvement? Using Typescript annotations for Ember classes

---

### Babel? Typescript?

---

### Babel

Takes future JS language features and turns it into current JS features

---

### Typescript

Can also emit current JS while providing type checking.

Supports a smaller set of transforms

---

TS playground https://bit.ly/2TUuljk

Babel playground https://bit.ly/2TRT2gC

---

![](04.png)

![](05.png)

---

![](06.png)
![](07.png)

---

![](08.png)

---

### Questions?
