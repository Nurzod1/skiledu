<template>
  <div class="footer">
    <div class="container">
      <div class="footer-wrapper">
        <div class="footer-logo-text">
          <div class="logo-wrapper">
            <img src="@/assets/images/footer-logo.svg" alt="" />
          </div>
          <h6 class="text-wrapper">
            Virtual Class <br />
            for Zoom
          </h6>
        </div>
        <form class="footer-subscribe">
          <p>Subscribe to get our Newsletter</p>
          <input type="email" name="" id="" placeholder="Your Email" />
          <button>Subscribe</button>
        </form>
        <div class="footer-links">
          <a href="">Careers</a>
          <a href="">Privacy Policy</a>
          <a href="">Terms & Conditions</a>
        </div>
        <p class="footer-class">© 2021 Class Technologies Inc.</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.footer {
  background: #252641;
  padding: 100px 0 30px 0;

  &-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
  }

  &-logo-text {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 60px;
  }
  .logo-wrapper {
    border-right: 2px solid #4a4b69;
    padding-right: 20px;

    img {
      width: 100%;
      height: 100%;
    }
  }

  .text-wrapper {
    font-weight: 600;
    font-size: 22px;
    line-height: 33px;
    color: #ffffff;
    margin-left: 15px;
  }

  &-subscribe {
    margin-bottom: 60px;

    p {
      font-weight: 500;
      font-size: 26px;
      line-height: 39px;
      text-align: center;
      letter-spacing: 0.04em;
      color: #b2b3cf;
      margin-bottom: 20px;
    }

    input {
      font-weight: normal;
      font-size: 20px;
      line-height: 30px;
      text-align: end;
      color: #83839a;
      background: transparent;
      padding: 15px 50px 15px 30px;
      margin-right: 20px;
      outline: none;
      border: 1px solid #83839a;
      box-sizing: border-box;
      border-radius: 80px;
    }

    button {
      padding: 14px 34px;
      font-weight: 600;
      font-size: 22px;
      line-height: 33px;
      color: #ffffff;
      background: linear-gradient(105.5deg, #545ae7 19.57%, #393fcf 78.85%);
      -webkit-box-shadow: 2px 4px 19px 3px rgba(65, 71, 214, 0.79);
      box-shadow: 2px 4px 19px 3px rgba(65, 71, 214, 0.79);
      border: none;
      border-radius: 60px;
      cursor: pointer;
    }
  }

  &-links {
    display: flex;
    align-items: center;
    margin-bottom: 20px;

    a {
      font-weight: normal;
      font-size: 22px;
      line-height: 33px;
      text-align: center;
      color: #b2b3cf;
      text-decoration: none;

      &:nth-child(2) {
        border-left: 1px solid #626381;
        border-right: 1px solid #626381;
        padding: 0 20px 0 20px;
        margin: 0 20px 0 20px;
      }
    }
  }

  &-class {
    font-weight: normal;
    font-size: 22px;
    line-height: 33px;
    text-align: center;
    color: #b2b3cf;
  }
}

@media screen and (max-width: 1199.98px) {
  .footer {
    &-subscribe {
      p {
        font-size: 23px;
      }

      input {
        font-size: 17px;
      }

      button {
        font-size: 20px;
      }
    }

    &-links {
      a {
        font-size: 20px;
      }
    }

    &-class {
      font-size: 15px;
    }
  }
}

@media screen and (max-width: 991.98px) {
  .footer {
    &-logo-text {
      margin-bottom: 50px;
    }

    .text-wrapper {
      font-size: 20px;
    }

    &-subscribe {
      p {
        font-size: 20px;
      }

      input {
        font-size: 15px;
      }

      button {
        font-size: 15px;
      }
    }

    &-links {
      a {
        font-size: 15px;
      }
    }

    &-class {
      font-size: 15px;
    }
  }
}

@media screen and (max-width: 767.98px) {
  .footer {
    padding: 60px 0 20px 0;

    &-logo-text {
      margin-bottom: 35px;
    }

    .text-wrapper {
      font-size: 20px;
    }

    &-subscribe {
      p {
        font-size: 15px;
      }

      input {
        padding: 10px 50px 10px 30px;
        font-size: 15px;
      }

      button {
        font-size: 15px;
        padding: 10px 34px;
      }
    }

    &-links {
      a {
        font-size: 15px;
      }
    }

    &-class {
      font-size: 15px;
    }
  }
}

@media screen and (max-width: 575.98px) {
  .footer {
    padding: 50px 0 20px 0;

    &-logo-text {
      margin-bottom: 35px;
    }

    .text-wrapper {
      font-size: 20px;
    }

    &-subscribe {
      display: flex;
      flex-direction: column;
      align-items: center;

      p {
        font-size: 15px;
      }

      input {
        margin-right: 0;
        margin-bottom: 15px;
        padding: 5px 30px 5px 20px;
        font-size: 15px;
      }

      button {
        font-size: 15px;
        padding: 5px 30px;
      }
    }

    &-links {
      a {
        font-size: 15px;
        &:nth-child(2) {
          padding: 0px 10px 0 10px;
          margin: 0 10px 0 10px;
        }
      }
    }

    &-class {
      font-size: 15px;
    }
  }
}
</style>
