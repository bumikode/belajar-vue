# 1. Tentang File vue

<div v-click>
Untuk project vue, kita bisa menggunakan file berformat <code>.html</code> apabila menggunakan CDN. Namun umumnya dalam pembuatan project, kita menggunakan file berformat <code>.vue</code></div>
<br/>
<div v-click>
Format <code>.vue</code> ini sebenernya tidak ada bedanya dengan penulisan html biasa. Namun memiliki kelebihan khusus yang ditambahkan dari vue itu sendiri</div>

---

# Isi dari file vue

Secara default dari vue sendiri, kita bisa mengisinya dengan 3 hal:

<div v-click>
1. Template HTML
<br/>
2. script javascript & vuejs
<br/>
3. css
</div>

<br/>
<div v-click>
contoh:

```js
<template></template>

<script setup></script>

<style></style>
```

</div>

---

# Fungsi-fungsi basic DOM dalam vue:
<div v-click>
1. Text interpolation / render value
```js
<div>{{ variable }}</div>
```
</div>
<br/>
<div v-click>
2. HTML interpolation / render html
```js
<div v-html="variable"></div>
```
</div>
<br/>
<div v-click>
3. Attribute binding
```js
<div v-bind:disabled="true"></div>
```
</div>
