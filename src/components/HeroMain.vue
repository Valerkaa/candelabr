<template>
  <div class="hero">
    <div class="hero-info">
      <div class="hero-info-text">
        <h2 class="hero-info-title">
          Lorem ipsum, dolor sit amet consectetur adipisicing.
        </h2>
        <span class="hero-info-description">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Facere
          maiores eveniet animi, magnam repellendus placeat.
        </span>
      
      </div>
      <a href="" class="hero-info-link">Lorem, ipsum.</a>
    </div>
  </div>
</template>

<script></script>

<style lang="scss" scoped>
@import url('https://fonts.cdnfonts.com/css/clash-display');
.hero {
  background: url("/img/main-hero.jpg");
  height: 704px;
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  padding-right: 80px;
  &-info {
    background: #fff;
    max-width: 630px;
    padding: 50px 55px;
    height: 444px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    &-title{
        font-family: 'Clash Display', sans-serif;
        font-weight: 400;
        line-height: 1.5;
        margin: 0 0 20px 0;
    }
    &-description{
        color: #5b5676;
        font-size: 18px;
    }
    &-link{
        color:#2a254b;
        text-decoration: none;
        &:hover{
            text-decoration: underline;
        }
    }
  }
}
</style>
