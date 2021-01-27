<template>
<div class="Tmp">
  <div class="Square Square--one" />
  <div class="Square Square--two" />
  </div>
</template>

<style>
.Tmp{
  display: inline-block;
  position: relative;
  overflow: hidden;
  height: 200px;
  width: 200px;
}

.Square {
  position:absolute;
  top: 0;
  left: 0;
  width: 0;
  height: 0;
}

.Square--one {
  border-top: 100px solid #449294;
  border-left: 100px solid #449294;
  border-right: 100px solid #449294;
  border-bottom: 100px solid #449294;
}

.Square--two {
  top: 0px;
  left: 70px;
  border-top: 70px solid #113044;
  border-left: 70px solid #113044;
  border-right: 70px solid #113044;
  border-bottom: 70px solid #113044;
}

</style>
