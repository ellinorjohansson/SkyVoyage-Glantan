<template>
  <button>Läs mer</button>
</template>

<style lang="scss" scoped>
button {
  font-family: $font-body;
  font-size: $font-size-button;
  width: 130px;
  height: 44px;
  border-radius: 8px;
  border: none;
  box-shadow: 0px 4px 4px 0px #00000040;
  background-color: $coral;
  color: black;

  &:disabled {
    background-color: #939393;
  }
}

@media screen and (min-width: 1024px) {
  button {
    width: 100px;
    height: 50px;

    &:hover {
      box-shadow: 0px 4px 4px 0px #00000040;
      background-color: #e5916d;
    }
  }
}
</style>
