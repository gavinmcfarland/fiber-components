<script>
  let className;
  export { className as class };
</script>

<style>
  .w-viewport {
    max-width: none !important;
    width: 100vw;

    position: relative;
    left: 50%;
    transform: translate(-50vw);
  }

  [class*="max-w"].w-viewport {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }

  [class*="max-w"].w-viewport > .wrapper {
    max-width: var(--max-width);
    display: block;
    box-sizing: content-box;
    width: 100vw;
    flex-shrink: 0;
    flex-basis: 100%;
  }
</style>

<div class="Section {className} max-w-6xl w-viewport border-t pt-12 pb-24">
  <div class="wrapper">
    <slot />
  </div>
</div>
