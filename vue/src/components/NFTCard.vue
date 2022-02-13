<template>
  <div class="nft__container">
    <article class="nft__card">
      <figure class="nft__img-container">
        <img
          class="nft__img-image"
          src="../assets/image-equilibrium.jpg"
          alt=""
        />
      </figure>
      <h1 class="nft__heading">Equilibrium #3429</h1>
      <p class="nft__subtitle">
        Our Equilibrium collection promotes balance and calm.
      </p>
      <section class="nft__details">
        <article class="nft__details-eth">
          <figure class="nft__details-eth-container">
            <img
              class="nft__details-eth-svg"
              src="../assets/icon-ethereum.svg"
              alt=""
            />
          </figure>
          <p class="nft__details-eth-price">0.041 ETH</p>
        </article>
        <article class="nft__details-time">
          <figure class="nft__details-time-container">
            <img
              class="nft__details-time-svg"
              src="../assets/icon-clock.svg"
              alt=""
            />
          </figure>
          <p class="nft__details-time-amount">3 days left</p>
        </article>
      </section>
      <div class="nft__line"></div>
      <section class="nft__creator">
        <figure class="nft__creator-img-container">
          <img
            class="nft__creator-img-avatar"
            src="../assets/image-avatar.png"
            alt=""
          />
        </figure>
        <p class="nft__creator-body">
          Creation of
          <span class="nft__creator-body--highlight">Jules Wyvern</span>
        </p>
      </section>
    </article>
  </div>
</template>

<style lang="scss">
:root {
  --background: hsl(217, 54%, 11%);
  --background--card: hsl(216, 50%, 16%);
  --line: hsl(215, 32%, 27%);
  --primary: hsl(178, 100%, 50%);
  --secondary: hsl(215, 51%, 70%);
  --white: hsl(0, 0%, 100%);
}

.nft {
  &__container {
    background-color: var(--background);
    min-height: 100vh;
    min-width: 100vw;
    display: flex;
    justify-content: center;
    align-items: center;
    box-sizing: border-box;
    padding: 1.5rem;
  }
  &__card {
    max-width: 350px;
    background-color: var(--background--card);
    padding: 1.5rem;
    border-radius: 0.9375rem;
  }
  &__img {
    &-container {
      display: flex;
      margin: 0;
    }
    &-image {
      border-radius: 0.625rem;
      height: 100%;
      width: 100%;
    }
  }
  &__heading {
    font-size: 1.375rem;
    font-weight: 600;
    color: var(--white);
    margin-bottom: 1rem;
  }
  &__subtitle {
    font-size: 1.125rem;
    font-weight: 300;
    line-height: 26px;
    letter-spacing: 1px;
    color: var(--secondary);
    margin-bottom: 1.5rem;
  }
  &__details {
    display: flex;
    justify-content: space-between;
    margin-bottom: 1.25rem;
    &-eth {
      display: flex;
      gap: 0.375rem;
      align-items: center;
      &-container {
        height: 1.125rem;
        width: 0.6875rem;
        display: flex;
        margin: 0;
      }
      &-svg {
        border-radius: 0.625rem;
        height: 100%;
        width: 100%;
      }
      &-price {
        font-weight: 600;
        color: var(--primary);
      }
    }
    &-time {
      display: flex;
      gap: 0.375rem;
      align-items: center;
      &-container {
        height: 1rem;
        width: 1rem;
        display: flex;
        margin: 0;
      }
      &-svg {
        border-radius: 0.625rem;
        height: 100%;
        width: 100%;
      }
      &-amount {
        font-weight: 600;
        color: var(--secondary);
      }
    }
  }
  &__line {
    width: 100%;
    border-bottom: 1px solid var(--secondary);
  }
  &__creator {
    display: flex;
    align-items: center;
    margin: 1rem 0;
    gap: 1rem;
    &-img {
      &-container {
        width: 2rem;
        height: 2rem;
        display: flex;
        margin: 0;
      }
      &-avatar {
        height: 100%;
        width: 100%;
        filter: drop-shadow(1px 0 0 white) drop-shadow(0 1px 0 white)
          drop-shadow(-1px 0 0 white) drop-shadow(0 -1px 0 white);
      }
    }
    &-body {
      color: var(--secondary);
      &--highlight {
        color: var(--white);
      }
    }
  }
}
</style>
