<template>
  <div class="skil-line">
    <div class="container">
      <div class="skil-line-wrapper">
        <div class="skil-title">
          <h3>What is <span>Skilline?</span></h3>
          <p>
            Skilline is a platform that allows educators to create online
            classes whereby they can store the course materials online; manage
            assignments, quizzes and exams; monitor due dates; grade results and
            provide students with feedback all in one place.
          </p>
        </div>
        <div class="skill-photos">
          <div class="skill-img">
            <img src="@/assets/images/skill-img-1.png" alt="" />
            <div class="skill-img-title">
              <h5>FOR INSTRUCTORS</h5>
              <button>Start a class today</button>
            </div>
          </div>
          <div class="skill-img">
            <img src="@/assets/images/skill-img.png" alt="" />
            <div class="skill-img-title">
              <h5>FOR Students</h5>
              <button>Enter access code</button>
            </div>
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
.skil-line {
  padding: 50px 0;

  .skil-title {
    margin-bottom: 80px;

    h3 {
      font-weight: 600;
      font-size: 44px;
      text-align: center;
      color: #2f327d;
      margin-bottom: 20px;

      span {
        color: #f48c06;
      }
    }

    p {
      font-weight: normal;
      font-size: 24px;
      text-align: center;
      color: #696984;
    }
  }

  .skill-photos {
    display: flex;
    justify-content: center;
    gap: 50px;

    .skill-img {
      position: relative;

      img {
        width: 100%;
        height: 100%;
      }
    }

    .skill-img-title {
      position: absolute;
      top: 35%;
      left: 22%;

      h5 {
        font-weight: 600;
        font-size: 32px;
        line-height: 48px;
        text-align: center;
        color: #ffffff;
        margin-bottom: 17px;
        text-transform: uppercase;
      }

      button {
        font-weight: 500;
        font-size: 22px;
        line-height: 33px;
        text-align: center;
        color: #ffffff;
        background: transparent;
        padding: 24px 38px;
        border: none;
        border: 1px solid #ffffff;
        border-radius: 50px;
        transition: 0.2s all;
        cursor: pointer;

        &:hover {
          border: 1px solid rgba(35, 189, 238, 0.9);
          background: rgba(35, 189, 238, 0.9);
        }
      }
    }
  }
}

@media screen and (max-width: 1199.98px) {
  .skil-line {
    .skil-title {
      h3 {
        font-size: 40px;
      }

      p {
        font-size: 20px;
      }
    }

    .skill-photos {
      .skill-img-title {
        h5 {
          font-size: 25px;
        }
      }
      button {
        padding: 20px 30px;
      }
    }
  }
}

@media screen and (max-width: 991.98px) {
  .skil-line {
    .skil-title {
      margin-bottom: 50px;

      h3 {
        font-size: 30px;
        margin-bottom: 15px;
      }

      p {
        font-size: 15px;
      }
    }

    .skill-photos {
      .skill-img-title {
        position: absolute;
        top: 27%;
        left: 15%;

        h5 {
          font-size: 20px;
          margin-bottom: 5px;
        }

        button {
          padding: 15px 25px;
        }
      }
    }
  }
}

@media screen and (max-width: 767.98px) {
  .skil-line {
    padding: 20px 0;

    .skil-title {
      margin-bottom: 30px;

      h3 {
        font-size: 25px;
        margin-bottom: 10px;
      }

      p {
        font-size: 12px;
      }
    }

    .skill-photos {
      .skill-img-title {
        position: absolute;
        top: 25%;
        left: 8%;

        h5 {
          font-size: 20px;
          margin-bottom: 0;
        }

        button {
          padding: 5px 10px;
        }
      }
    }
  }
}

@media screen and (max-width: 575.98px) {
  .skil-line {
    padding: 20px 0;

    .skil-title {
      margin-bottom: 30px;

      h3 {
        font-size: 25px;
        margin-bottom: 10px;
      }

      p {
        font-size: 12px;
      }
    }

    .skill-photos {
      display: flex;
      flex-direction: column;
      .skill-img-title {
        position: absolute;
        top: 25%;
        left: 8%;

        h5 {
          font-size: 20px;
          margin-bottom: 0;
        }

        button {
          padding: 5px 10px;
        }
      }
    }
  }
}
</style>
