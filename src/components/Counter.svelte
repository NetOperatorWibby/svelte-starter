<script lang="ts">
  export let value: number = 0;
  export let step: number = 1;
</script>

<section>
  <slot>Default Counter</slot>

  <div>
    {value}

    <button on:click={() => (value += step)}>+</button>
    <button on:click={() => (value -= step)}>-</button>
  </div>
</section>
