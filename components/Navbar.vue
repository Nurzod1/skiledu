<template>
  <div class="navbar">
    <div class="container">
      <div class="navbar-wrapper">
        <div class="wrapper-burger" @click="$emit('isOpen')">
          <div class="burger"></div>
          <div class="burger"></div>
          <div class="burger"></div>
          <div class="burger"></div>
        </div>
        <div class="logo-wrapper">
          <img src="@/assets/images/logo.png" alt="" />
          <h4 class="logo-text">Skilline</h4>
        </div>
        <div class="navbar-links">
          <div class="navbar-menu">
            <a href="">Home</a>
            <a href="">Carrers</a>
            <a href="">Blog</a>
            <a href="">About Us</a>
          </div>
          <div class="navbar-reg">
            <a class="log right" href="">Log in</a>
            <a class="log" href="">Sign Up</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.navbar {
  padding: 15px 0;

  &-wrapper {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .wrapper-burger {
    display: flex;
    flex-direction: column;
    display: none;

    .burger {
      width: 32px;
      height: 2px;
      background: #ffffff;
      margin-bottom: 5px;
    }
  }

  .logo-wrapper {
    position: relative;

    img {
      width: 100%;
      height: 100%;
    }

    .logo-text {
      position: absolute;
      top: 15%;
      left: 40%;
      font-style: normal;
      font-weight: 700;
      font-size: 32px;
      color: #113c49;
    }
  }

  &-links {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 70%;
  }

  &-menu {
    display: flex;
    justify-content: space-between;
    width: 65%;

    a {
      font-weight: normal;
      font-size: 22px;
      color: #252641;
      text-decoration: none;
      transition: 0.3s all;

      &:hover {
        transform: translateY(-10px);
      }
    }
  }

  .navbar-reg {
    display: flex;
    align-items: center;
    margin-left: 20px;

    .log {
      border: 1px solid #ffffff;
      background: #ffffff;
      box-shadow: 0px 20px 24px rgba(0, 0, 0, 0.03);
      border-radius: 80px;
      padding: 10px 40px;
      text-decoration: none;
      white-space: nowrap;

      &.right {
        margin-right: 35px;
      }

      &:hover {
        background: #f48c06;
        color: #ffffff;
      }
    }
  }
}

@media screen and (max-width: 1199.98px) {
  .navbar {
    &-links {
      a {
        font-size: 17px;
      }
    }

    .navbar-reg {
      .log {
        padding: 3px 25px;
      }
    }
  }
}

@media screen and (max-width: 991.98px) {
  .navbar {
    .logo-wrapper {
      width: 55px;
      height: 55px;

      .logo-text {
        font-size: 25px;
      }
    }

    &-links {
      a {
        font-size: 14px;
      }
    }

    .navbar-reg {
      margin-left: 15px;
      .log {
        padding: 3px 20px;
      }
    }
  }
}

@media screen and (max-width: 767.98px) {
  .navbar {
    &-wrapper {
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-direction: row-reverse;
      padding: 10px 8px;
    }

    .wrapper-burger {
      display: block;
    }

    .logo-wrapper {
      width: 45px;
      height: 45px;

      .logo-text {
        font-size: 20px;
      }
    }

    &-links {
      display: none;

      a {
        font-size: 14px;
      }
    }

    .navbar-reg {
      display: none;
      margin-left: 15px;

      .log {
        padding: 3px 20px;
      }
    }
  }
}
</style>
