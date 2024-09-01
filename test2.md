.split-layout {
  display: flex;
  flex-direction: column;
}

@media screen and (min-width: 30em) {
  .split-layout {
    flex-direction: row;
    align-items: stretch;
  }
}

.split-layout__item {
  flex: 1;
}

@media screen and (min-width: 30em) {
  .split-layout__item {
    padding-left: 1em;
  }
  .split-layout__item:first-child {
    padding: 0;
  }
}

.split-layout__divider {
  display: flex;
  flex-direction: row;
  align-items: center;
}

@media screen and (min-width: 30em) {
  .split-layout__divider {
    flex-direction: column;
  }
}

.split-layout__label {
  padding: 1em;
}

.split-layout__rule {
  flex: 1;
  border-style: solid;
  border-color: rgba(255, 255, 255, 0.3);
  border-width: 1px 0 0 0;
}

@media screen and (min-width: 30em) {
  .split-layout__rule {
    border-width: 0 1px 0 0;
  }
}


/*	=DEMO STYLES
--------------------------------------------------------------------*/

html {
  padding: 2em;
  background: #3B4558;
  color: #fff;
}

<div class="wrapper">
  <div class="split-layout">
    <div class="split-layout__item">
      <h2>Navigation</h2>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Id eos esse voluptates cupiditate expedita inventore, temporibus? In beatae hic tenetur molestiae facilis illo neque esse repellendus harum. A, consequatur, labore.
      </p>
    </div>
    <div class="split-layout__divider">
      <div class="split-layout__rule"></div>
      <div class="split-layout__rule"></div>
    </div>
    <div class="split-layout__item">
      <h2>Content</h2>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Id eos esse voluptates cupiditate expedita inventore, temporibus?
      </p>
    </div>
  </div>
</div>