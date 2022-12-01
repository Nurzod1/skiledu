<template>
  <div class="clients">
    <div class="container">
      <div class="clients-wrapper">
        <h3 class="clients-title">Trusted by 5,000+ Companies Worldwide</h3>
        <div class="icons-main-wrapper">
          <div class="icon-wrapper" v-for="(s, i) in icons" :key="i">
            <img :src="s.imgUrl" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Clients",
  data() {
    return {
      icons: [
        {
          imgUrl: require("@/assets/images/google.png"),
        },
        {
          imgUrl: require("@/assets/images/netflix.png"),
        },
        {
          imgUrl: require("@/assets/images/airbnb.png"),
        },
        {
          imgUrl: require("@/assets/images/amazon.png"),
        },
        {
          imgUrl: require("@/assets/images/facebook.png"),
        },
        {
          imgUrl: require("@/assets/images/grab-logo.png"),
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.clients {
  padding: 50px 0;

  &-title {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 33px;
    font-weight: 500;
    font-size: 28px;
    line-height: 160%;
    letter-spacing: 0.02em;
    color: #696984;
  }

  .icons-main-wrapper {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .icon-wrapper {
    width: auto;
    height: 50px;

    img {
      width: 100%;
      height: 100%;
      filter: grayscale(10);
      transition: 0.2s all;

      &:hover {
        filter: grayscale(0);
      }
    }
  }
}

@media screen and (max-width: 1199.98px) {
  .clients {
    .icon-wrapper {
      width: auto;
      height: 40px;
    }
  }
}

@media screen and (max-width: 991.98px) {
  .clients {
    &-title {
      font-size: 20px;
      margin-bottom: 25px;
    }

    .icon-wrapper {
      width: auto;
      height: 30px;
    }
  }
}

@media screen and (max-width: 767.98px) {
  .clients {
    &-title {
      font-size: 17px;
      margin-bottom: 25px;
    }

    .icon-wrapper {
      width: auto;
      height: 25px;
    }
  }
}

@media screen and (max-width: 575.98px) {
  .clients {
    &-title {
      font-size: 17px;
      margin-bottom: 25px;
    }

    .icons-main-wrapper {
      gap: 10px;
      flex-wrap: wrap;
      justify-content: flex-start;
    }

    .icon-wrapper {
      width: auto;
      height: 25px;
    }
  }
}
</style>
