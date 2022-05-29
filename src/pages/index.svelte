<script lang="ts">
  import Counter from '../lib/Counter.svelte'
  import Go from '../lib/Go.svelte'
  import init from '../lib/example.wasm'

  init().then((exports) => {
    let r = exports.add(3, 4)
    console.log("result of add(3,4) is", r)
  })
</script>

<button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
  Button
</button>

<button class="btn btn-warning">Warning</button>

<Counter />

<br/>

<Go />

<br />

<a href="/about">About</a>

<br />
