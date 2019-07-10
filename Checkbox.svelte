<label>
  <input type="checkbox" />
  <div class="checkbox"><div class="checkmark"></div></div>
  <div class="checkboxLabel"><slot></slot></div>
</label>

<style>
  input + :global(.Label) {
    color: red;
  }
  .checkbox {
    width: 24px;
    height: 24px;
    background-color: color-mod(YELLOW a(5%));
    border: inside 2px solid YELLOW;
    border-radius: 4px;
    display: inline-block;
    vertical-align: middle;
  }
  .checkboxLabel {
    display: inline-block;
    vertical-align: middle;
  }
  label {
    display: flex;
    line-height: 1;
    align-items: center;
    cursor: pointer;
  }
  label > :not(:last-child) {
    margin-right: 1.5sp;
  }
  /* Hide the native input */
  input {
    padding: 0;
    margin: 0;
    border: none;
    position: absolute;
    -webkit-appearance: unset;
  }
  input + span {
    display: block;
    width: 24px;
    height: 24px;
    background: green;
  }
  /* Checked */
  input:checked + .checkbox {
    background-color: red;
  }
  input:focus {
    outline: none;
  }
  /* input:focus + .checkbox {
		outline: 3px solid pink;
	} */
</style>
