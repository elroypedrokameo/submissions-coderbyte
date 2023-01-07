<script setup>
</script>

<template>
  <div class="body">
    <div class="container">
      <div class="items">
        <div class="item-1">
          ITEM 1
        </div>
        <div class="item-234">
          <div class="item-4">ITEM 4</div>
          <div class="item-23">
            <div class="item-2">ITEM 2</div>
            <div class="item-3">ITEM 3</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
@media screen and (max-width: 768px) {
  .items {
    display: flex;
    flex-direction: column;
  }
  .item-4{
    order: 2;
  }
}

.body {
  background-color: #ECECEC;
  min-height: 100vh;
  min-width: 100vw;
  display: flex;
  justify-content: center;
  align-items: center;
}
.container {
  background-color: #FF7573;
  height: 80vh;
  width: 80vw;
  border-radius: 20px;
  display: grid;
  place-items: center;
}

.items {
  height: 90%;
  width: 90%;
  display: flex;
  justify-content: center;
  gap: 1rem;
  font-weight: bold;
}

.item-1, .item-2, .item-3, .item-4 {
  border-radius: 20px;
  display: grid;
  place-items: center;
}

.item-1 {
  background-color: #7699FF;
  height: 100%;
  width: 100%;
}
.item-4 {
  background-color: #77FFFB;
}
.item-2 {
  background-color: #75FFA7;
}
.item-3 {
  background-color: #EEFF75;
}
.item-23{
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 1rem;
}
.item-234 {
  display: grid;
  gap: 1rem;
  height: 100%;
  width: 100%;
}
</style>
