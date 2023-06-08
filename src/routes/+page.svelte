<script lang="ts">
</script>

<main>
  <div class="card">
    <img src="./assets/images/image-equilibrium.jpg" alt="card representation">
    <div class="thumbnail">
      <img src="./assets/images/icon-view.svg" alt="white eye icon">
    </div>
  </div>
  <h1>Equilibrium #3429</h1>
  <p>Our Equilibrium collection promotes balance and calm.</p>
  <div class="infos-container">
    <div class="info price">
      <img src="./assets/images/icon-ethereum.svg" alt="ethereum logo">
      <h2>0.041 ETH</h2>
    </div>
    <div class="info timer">
      <img src="./assets/images/icon-clock.svg" alt="clock icon">
      <p>3 days left</p>
    </div>
  </div>
  <div class="line"></div>
  <div class="creator-container">
    <img src="./assets/images/image-avatar.png" alt="card's creator">
    <p>Creation of <span>Jules Wyvern</span></p>
  </div>
</main>
<footer class="attribution">
  Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a> | 
  <a href="https://github.com/anespoul34" target="_blank">Coded</a> by <a href="https://www.arthurnespoulous.com" target="_blank">AN</a>. 
</footer>

<style lang="scss">
  main {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: flex-start;
    width: 360px;
    height: 600px;
    padding: 20px;
    border-radius: 10px;
    background-color: $medium;
    box-shadow: 0 10px 30px -10px $black;

    .card {
      width: 320px;
      height: 320px;
      cursor: pointer;
      position: relative;
      width: 100%;
      border-radius: 10px;
      overflow: hidden;

      img {
        width: 100%;
        z-index: 1;
      }
      .thumbnail {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        opacity: 0;
        background: hsla(178, 100%, 50%, 0.5);
        transition: all 0.2s ease-in-out;
        z-index: 2;

        img {
          width: 60px;
        }
      }
      &:hover .thumbnail {
        opacity: 1;
      }
    }
    p {
      line-height: 1.4;
    }
    .infos-container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      width: 100%;

      .info {
        display: flex;
        justify-content: flex-start;
        align-items: center;

        img {
          margin-right: 8px;
        }
      }
    }
    .line {
      width: 100%;
      height: 1px;
      background-color: $light;
    }
    .creator-container {
      display: flex;
      justify-content: flex-start;
      align-items: center;

      img {
        border: 1px solid $white;
        border-radius: 50%;
        width: 30px;
        margin-right: 10px;
      }
      span {
        cursor: pointer;
      }
    }
  }
</style>