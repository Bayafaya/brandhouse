<template>
      <div class="brands">
      <div class="header__of__products">
        <span>Топ бренды</span>
        <button class="all_products">Все бренды</button>
      </div>
      <div class="brand__grid">
        <div class="brand__item">
          <div class="brand__img">
            <img src="../image/makfa.png" alt="card" />
          </div>
          <span>Makfa</span>
        </div>

        <div class="brand__item">
          <div class="brand__img">
            <img src="../image/jacobs.png" alt="card" />
          </div>
          <span>Jacobs</span>
        </div>

        <div class="brand__item">
          <div class="brand__img">
            <img src="../image/milka.png" alt="card" />
          </div>
          <span>Milka</span>
        </div>

        <div class="brand__item">
          <div class="brand__img">
            <img src="../image/pringles.png" alt="card" />
          </div>
          <span>Pringles</span>
        </div>

        <div class="brand__item">
          <div class="brand__img">
            <img src="../image/dan.png" alt="card" />
          </div>
          <span>Dansukker</span>
        </div>

        <div class="brand__item">
          <div class="brand__img">
            <img src="../image/alpen.png" alt="card" />
          </div>
          <span>Alpen Gold</span>
        </div>

        <div class="brand__item">
          <div class="brand__img">
            <img src="../image/candy.png" alt="card" />
          </div>
          <span>Gandy Gold</span>
        </div>

        <div class="brand__item">
          <div class="brand__img">
            <img src="../image/snickers.png" alt="card" />
          </div>
          <span>Snickers</span>
        </div>
      </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.brands {
  padding: 24px 16px;
}
.brand__grid {
  display: grid;
  grid-template: repeat(2, 1fr) / repeat(4, 1fr);
  grid-column-gap: 12px;
  grid-row-gap: 24px;
  padding: 24px 0;
}
.brand__item {
  width: 72px;
  font-family: "SF UI Display";
  font-style: normal;
  font-weight: 400;
  font-size: 11px;
  line-height: 12px;
  text-align: center;
  margin: 0 auto;
}
.brand__img {
  border-radius: 50%;
  background: #f2f2f7;
  margin-bottom: 8px;
}
.brand__item img {
  width: 100%;
}
</style>