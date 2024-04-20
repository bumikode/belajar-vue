---
titleTemplate: "%s - Fundamental"
---

# Fundamental

## Apa itu Vuejs?

- Vuejs adalah library javascript untuk membangun user interface dengan tetap menggunakan html, css, dan js.
- Perbedaan vuejs dan html biasa:

1. Declarative rendering — menampilkan html sesuai dengan state javascript
2. Reactivity — vue akan memantau state javascript agar ketika perubahan terjadi, maka DOM bisa di update langsung sesuai dengan state yg diubah

---

# Contoh code reactive menggunakan javascript

<iframe src="https://codesandbox.io/embed/fyyjr7?view=editor+%2B+preview&module=%2Findex.html"
    class="w-full h-[400px]"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

---

# Contoh code reactive menggunakan Vuejs

<iframe src="https://codesandbox.io/embed/2sd9gk?view=editor+%2B+preview&module=%2Fsrc%2FApp.vue"
    class="w-full h-[400px]"
     title="thirsty-perlman-2sd9gk"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

---

## layout: center

# Baris code menjadi lebih kecil

````md magic-move
```js
<body>
  <button onclick="add()">Click me</button>

  <div id="hasil1"></div>
  <div id="hasil2"></div>

  <script>
    let num = 0;
    document.querySelector("#hasil1").innerHTML = `${num}`;
    document.querySelector("#hasil2").innerHTML = `${num} ditambah 2 = ${
      num + 2
    }`;

    function add() {
      num++;
      document.querySelector("#hasil1").innerHTML = `${num}`;
      document.querySelector("#hasil2").innerHTML = `${num} ditambah 2 = ${
        num + 2
      }`;
    }
  </script>
</body>

```

```js
<template>
  <button @click="num++">Click me</button>
  <div>{{ num }}</div>
  <div>{{ num }} ditambah 2 = {{ num + 2 }}</div>
</template>

<script setup>
import { ref } from "vue";
const num = ref(0);
</script>
```
````

---

## layout: two-cols-header

# 2 Macam cara menggunakan vuejs

::left::

<div v-click class="-translate-y-40 m-3">
<div v-after class="text-2xl">1. Option API</div>
```js
export default {
  data: {
    num: 0,
  },
  methods: {
    add() {
      this.num++;
    }
  }
}
```
</div>

::right::

<div v-click class="-translate-y-40 m-3">
<div v-after class="text-2xl">2. Composition API</div>
```js
import {ref} from "vue";
const num = ref(0);
function add() {
  num.value++;
}
```
</div>

---

# Pembuatan project vuejs

<v-click>Untuk membuat project vuejs, ada beberapa opsi yang bisa kita gunakan:</v-click>
<br/>
<v-click>1. Vite template</v-click>
<br/>
<v-click>2. CDN</v-click>
<br/>
<v-click>3. Nuxtjs</v-click>
<br/>
<v-click>4. Astro</v-click>
<br/>
<v-click>5. Vuepress</v-click>

---

# Kurikulum yang akan dipelajari

<br/>
<div class="-translate-y-8">
<div v-click>1. Tentang file vue</div>
<div v-after>2. Fundamental reactive</div>
<div v-after>3. Event handling</div>
<div v-after>4. Conditional rendering</div>
<div v-after>5. List rendering</div>
<div v-after>6. Class dan style binding + bikin project</div>
<div v-after>7. Computed properties & watcher</div>
<div v-after>8. Form input binding</div>
<div v-after>9. Lifecycle hooks + bikin project</div>
<div v-after>10. Template ref</div>
<div v-after>11. Components</div>
<div v-after>12. Props & event</div>
<div v-after>13. Slots</div>
<div v-after>14. V-model component</div>
<div v-after>15. Composable</div>
<div v-after>16. Bikin project akhir</div>
</div>
