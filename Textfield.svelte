<style>
  input {
    padding: 2.5sp 2sp;
    width: 100%;
    box-sizing: border-box;
    caret-color: GREEN;
  }
  label {
    display: block;
  }
  /* .help-text {
		padding-top: 0.5sp;
	} */
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
  }
  input {
    background: transparent;
    background-color: color-mod(YELLOW a(5%));
    border: inside 2px solid YELLOW;
    border-radius: 4px;
    color: inherit;
    line-height: 3sp;
  }
  .checkbox {
    width: 24px;
    height: 24px;
    background-color: color-mod(YELLOW a(20%));
    border: inside 2px solid YELLOW;
    border-radius: 4px;
    display: inline-block;
    vertical-align: middle;
  }
  .checkboxLabel {
    display: inline-block;
    vertical-align: middle;
  }
  input:focus {
    outline: none;
  }
  /* input:focus + .checkbox {
		outline: 3px solid pink;
	} */
</style>

<label>
  <div class="label">{label}</div>
  <input type="text" />
  <!-- <div class="help-text"><slot/></div> -->
</label>
