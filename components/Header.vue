<template>
  <div class="header">
    <div class="container">
      <div class="header-wrapper">
        <Sidebar :active="isActive" />
        <Navbar @isOpen="isActive = !isActive" />
        <div class="intro">
          <div class="intro-content">
            <h1 class="intro-title">
              <span>Studying</span> Online is now much easier
            </h1>
            <p class="intro-subtitle">
              Skilline is an interesting platform that will teach you in more an
              interactive way
            </p>
            <div class="intro-btns">
              <button class="join">Join for free</button>
              <button class="play">
                <img src="@/assets/images/play.svg" alt="" />
              </button>
              <span>Watch how it works</span>
            </div>
          </div>

          <div class="intro-image">
            <img
              class="intro-image-item"
              src="@/assets/images/header-pic.png"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Sidebar from "@/components/Sidebar";
import Navbar from "@/components/Navbar.vue";

export default {
  name: "Header",

  components: {
    Navbar,
    Sidebar,
  },

  data() {
    return {
      isActive: false,
    };
  },
};
</script>

<style lang="scss" scoped>
.header {
  background-color: #fff2e1;
  min-height: 100vh;
  display: flex;

  &-wrapper {
    display: flex;
    flex-direction: column;
    height: 100%;
  }

  .intro {
    display: flex;
    align-items: center;
    justify-content: center;
    flex: 1;

    &-content {
      display: flex;
      flex-direction: column;
      flex: 1;
    }

    &-title {
      color: #2f327d;
      font-size: 45px;
      font-weight: 700;
      margin-bottom: 24px;

      span {
        color: #f48c06;
      }
    }

    &-image {
      flex: 1;
      display: flex;

      &-item {
        width: 100%;
        height: 100%;
        object-fit: contain;
      }
    }

    &-subtitle {
      font-family: Nun;
      font-size: 24px;
      color: #464646;
      margin-bottom: 40px;
    }

    &-btns {
      display: flex;
      align-items: center;

      .join {
        color: #ffffff;
        background: #f48c06;
        font-weight: 600;
        font-size: 20px;
        padding: 15px 35px;
        border: none;
        border-radius: 80px;
        white-space: nowrap;
        cursor: pointer;
      }

      .play {
        width: 80px;
        height: 80px;
        background: #ffffff;
        margin: 0 32px 0 40px;
        padding: 24px 22px 24px 26px;
        border: none;
        border-radius: 50%;
        box-shadow: 2px 20px 60px rgba(61, 155, 185, 0.1);
        cursor: pointer;
        transition: 0.3s all;

        &:hover {
          transform: scale(1.1);
        }

        img {
          width: 100%;
          height: 100%;
        }
      }

      span {
        font-weight: normal;
        font-size: 24px;
        line-height: 36px;
        color: #252641;
      }
    }
  }
}

@media screen and (max-width: 1199.98px) {
  .header {
    .intro {
      &-btns {
        .join {
          font-size: 15px;
          padding: 15px 35px;
        }

        .play {
          width: 70px;
          height: 70px;
        }
      }
    }
  }
}

@media screen and (max-width: 991.98px) {
  .header {
    .intro {
      padding: 50px 0;

      &-title {
        font-size: 35px;
        font-weight: 600;
        margin-bottom: 20px;
      }

      &-subtitle {
        margin-bottom: 35px;
      }

      &-btns {
        .join {
          font-size: 15px;
          padding: 15px 35px;
        }

        .play {
          width: 70px;
          height: 70px;
        }
      }

      &-image {
        display: none;
      }
    }
  }
}

@media screen and (max-width: 575.98px) {
  .header {
    .intro {
      padding: 50px 0;

      &-title {
        font-size: 30px;
        font-weight: 600;
        margin-bottom: 15px;
      }

      &-subtitle {
        font-size: 20px;
        margin-bottom: 25px;
      }

      &-btns {
        display: flex;
        flex-direction: column;

        .join {
          font-size: 15px;
          padding: 15px 35px;
          margin-bottom: 15px;
        }

        .play {
          display: flex;
          align-items: center;
          width: 70px;
          height: 70px;
        }
        span {
          font-size: 15px;
        }
      }

      &-image {
        display: none;
      }
    }
  }
}
</style>
