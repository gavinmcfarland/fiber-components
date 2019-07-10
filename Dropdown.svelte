<style>
  select {
    padding: 2.5sp 2sp;
    width: 100%;
    caret-color: GREEN;
    background-color: color-mod(YELLOW a(5%));
    border: inside 2px solid YELLOW;
    border-radius: 4px;
    color: inherit;
    line-height: 3sp;
  }
  .label {
    margin-bottom: -7px;
    background-color: color-mod(YELLOW blend(white 95%));
    position: relative;
    display: table;
    line-height: 1;
    padding: 0px 0.5sp;
    margin-left: 16px;
    font-size: 1fs;
    letter-spacing: 0.03em;
    user-select: none;
    pointer-events: none;
  }
</style>

<div class="label">{label}</div>
<select class="Dropdown">
  <slot></slot>
</select>
