<template>
  <div class="class-room">
    <div class="container">
      <div class="class-wrapper">
        <div class="class-title">
          <div class="big-round">
            <img src="@/assets/images/big-round.svg" alt="" />
          </div>
          <div class="small-round">
            <img src="@/assets/images/small-round.svg" alt="" />
          </div>
          <h3>
            Everything you can do in a physical classroom,
            <span>you can do with Skilline</span>
          </h3>
          <p>
            Skilline’s school management software helps traditional and online
            schools manage scheduling, attendance, payments and virtual
            classrooms all in one secure cloud-based system.
          </p>
          <a href="#">Learn More</a>
        </div>
        <div class="class-photo">
          <img src="@/assets/images/video-img.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.class-room {
  padding: 50px 0;

  .class-wrapper {
    display: flex;
    gap: 20px;
  }

  .class-title {
    display: flex;
    flex-direction: column;
    width: 100%;
    margin-right: 50px;
    position: relative;

    .big-round {
      width: 73px;
      height: 73px;
      position: absolute;
      top: -3%;
      left: -4%;
      z-index: -1;

      img {
        width: 100%;
        height: 100%;
      }
    }
    .small-round {
      width: 30px;
      height: 30px;
      position: absolute;
      right: 8%;
      bottom: 20%;
      z-index: -1;

      img {
        width: 100%;
        height: 100%;
      }
    }

    h3 {
      font-weight: 500;
      font-size: 36px;
      color: #2f327d;

      span {
        color: #f48c06;
      }
    }

    p {
      font-weight: normal;
      font-size: 24px;
      color: #696984;
      margin: 30px 0 30px 0;
    }

    a {
      font-weight: normal;
      font-size: 22px;
      text-decoration-line: underline;
      color: #696984;
    }
  }

  .class-photo {
    display: flex;
    align-items: center;

    img {
      width: 100%;
      height: auto;
    }
  }
}

@media screen and (max-width: 1199.98px) {
  .class-room {
    .class-title {
      h3 {
        font-size: 30px;
      }

      p {
        font-size: 20px;
      }

      a {
        font-size: 20px;
      }
    }
  }
}

@media screen and (max-width: 991.98px) {
  .class-room {
    .class-title {
      margin-right: 25px;

      h3 {
        font-size: 25px;
      }

      p {
        font-size: 15px;
        margin: 15px 0 15px 0;
      }

      a {
        font-size: 15px;
      }
    }
  }
}

@media screen and (max-width: 767.98px) {
  .class-room {
    .class-wrapper {
      display: flex;
      flex-direction: column;
    }

    .class-title {
      margin-right: 25px;

      h3 {
        font-size: 25px;
      }

      p {
        font-size: 15px;
        margin: 15px 0 15px 0;
      }

      a {
        font-size: 15px;
      }
    }
  }
}

@media screen and (max-width: 575.98px) {
  .class-room {
    .class-wrapper {
      display: flex;
      flex-direction: column;
    }

    .class-title {
      margin-right: 25px;

      h3 {
        font-size: 25px;
        text-align: center;
      }

      p {
        text-align: center;
        font-size: 15px;
        margin: 15px 0 15px 0;
      }

      a {
        font-size: 15px;
      }

      .big-round {
        display: none;
      }

      .small-round {
        display: none;
      }
    }
  }
}
</style>
