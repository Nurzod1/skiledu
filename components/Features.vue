<template>
  <div class="features">
    <div class="container">
      <div class="features-wrapper">
        <div class="features-title">
          <h3>Our <span>Features</span></h3>
          <p>
            This very extraordinary feature, can make learning activities more
            efficient
          </p>
        </div>
        <div class="features-interface">
          <div class="interface-img">
            <img src="@/assets/images/features-1.png" alt="" />
          </div>
          <div class="interface-info">
            <h5 class="interface-title">
              A <span>user interface</span> designed for the classroom
            </h5>
            <div class="interface-curve">
              <div class="icon">
                <img src="@/assets/images/interface-1.svg" alt="" />
              </div>
              <p class="interface-icon-text">
                Teachers don’t get lost in the grid view and have a dedicated
                Podium space.
              </p>
            </div>
            <div class="interface-curve">
              <div class="icon">
                <img src="@/assets/images/interface-2.svg" alt="" />
              </div>
              <p class="interface-icon-text">
                TA’s and presenters can be moved to the front of the class.
              </p>
            </div>
            <div class="interface-curve">
              <div class="icon">
                <img src="@/assets/images/interface-3.svg" alt="" />
              </div>
              <p class="interface-icon-text">
                Teachers can easily see all students and class data at one time.
              </p>
            </div>
          </div>
        </div>
        <div class="tools">
          <div class="tools-title">
            <h5><span>Tools </span> For Teachers And Learners</h5>
            <p>
              Class has a dynamic set of teaching tools built to be deployed and
              used during class. Teachers can handout assignments in real-time
              for students to complete and submit.
            </p>
          </div>
          <div class="tools-photo">
            <img src="@/assets/images/features-2.png" alt="" />
          </div>
        </div>
        <div class="tools reverse">
          <div class="tools-title">
            <h5>Assessments, <span>Quizzes,</span> Tests</h5>
            <p>
              Easily launch live assignments, quizzes, and tests. Student
              results are automatically entered in the online gradebook.
            </p>
          </div>
          <div class="tools-photo">
            <img src="@/assets/images/features-3.png" alt="" />
          </div>
        </div>
        <div class="tools">
          <div class="tools-title">
            <h5><span>Class Management</span> Tools for Educators</h5>
            <p>
              Class has a dynamic set of teaching tools built to be deployed and
              used during class. Teachers can handout assignments in real-time
              for students to complete and submit.
            </p>
          </div>
          <div class="tools-photo">
            <img src="@/assets/images/features-4.png" alt="" />
          </div>
        </div>
        <div class="tools reverse">
          <div class="tools-title">
            <h5>One-on-One <span>Discussions</span></h5>
            <p>
              Teachers and teacher assistants can talk with students privately
              without leaving the Zoom environment.
            </p>
          </div>
          <div class="tools-photo">
            <img src="@/assets/images/features-5.png" alt="" />
          </div>
        </div>
        <div class="features-btn">
          <button>See more features</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.features {
  &-wrapper {
    display: flex;
    flex-direction: column;
  }

  &-title {
    h3 {
      font-weight: bold;
      font-size: 36px;
      line-height: 180%;
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
      line-height: 180%;
      text-align: center;
      color: #696984;
    }
  }

  &-interface {
    display: flex;
    padding: 50px 0;
  }

  .interface-img {
    width: 100%;
    display: flex;
    align-items: center;
    img {
      width: 100%;
      height: auto;
    }
  }

  .interface-info {
    width: 100%;
  }

  .interface-title {
    margin-bottom: 50px;
    font-weight: 600;
    font-size: 40px;
    line-height: 160%;
    color: #2f327d;

    span {
      color: #f48c06;
    }
  }

  .interface-curve {
    display: flex;
    align-items: center;

    &:nth-child(3) {
      margin: 40px 0 40px 0;
    }
  }

  .icon {
    background: #fbfbfb;
    border-radius: 50%;
    box-shadow: 0px 15px 44px rgba(13, 15, 28, 0.12);
    width: 60px;
    height: 60px;
    display: flex;
    justify-content: center;
    padding: 15px;
    margin-right: 40px;
  }
  .interface-icon-text {
    font-weight: normal;
    font-size: 22px;
    line-height: 180%;
    color: #696984;
  }

  .tools {
    display: flex;
    align-items: center;

    &.reverse {
      display: flex;
      align-items: center;
      flex-direction: row-reverse;
    }

    &-title {
      padding: 50px;
      width: 50%;

      h5 {
        font-weight: 600;
        font-size: 40px;
        line-height: 160%;
        color: #2f327d;
        margin-bottom: 20px;

        span {
          color: #f48c06;
        }
      }

      p {
        font-weight: normal;
        font-size: 22px;
        color: #696984;
      }
    }

    &-photo {
      width: 50%;

      img {
        width: 100%;
        height: 100%;
      }
    }
  }
  &-btn {
    display: flex;
    align-items: center;
    justify-content: center;

    button {
      color: #f48c06;
      background: transparent;
      font-family: Nun;
      font-weight: normal;
      font-size: 24px;
      line-height: 180%;
      padding: 19px 38px;
      border: none;
      border: 1px solid #f48c06;
      border-radius: 40px;
      transition: 0.2s all;
      cursor: pointer;

      &:hover {
        color: #ffffff;
        background: #f48c06;
      }
    }
  }
}

@media screen and (max-width: 1199.98px) {
  .features {
    &-title {
      h3 {
        font-size: 30px;
        margin-bottom: 10px;
      }

      p {
        font-size: 20px;
      }
    }

    .interface-title {
      font-size: 30px;
      margin-bottom: 40px;
    }

    .interface-curve {
      &:nth-child(3) {
        margin: 30px 0 30px 0;
      }
    }

    .tools {
      &-title {
        h5 {
          font-size: 30px;
        }

        p {
          font-size: 20px;
        }
      }
    }

    &-btn {
      button {
        font-size: 20px;
        padding: 15px 30px;
      }
    }
  }
}

@media screen and (max-width: 991.98px) {
  .features {
    &-title {
      h3 {
        margin-bottom: 5px;
      }

      p {
        font-size: 20px;
      }
    }

    &-interface {
      padding: 30px 0;
    }

    .interface-title {
      font-size: 20px;
      margin-bottom: 15px;
    }

    .interface-curve {
      &:nth-child(3) {
        margin: 20px 0 20px 0;
      }

      .icon {
        width: 55px;
        height: 55px;
        margin-right: 30px;
      }
    }

    .interface-icon-text {
      font-size: 15px;
    }

    .tools {
      &-title {
        h5 {
          font-size: 25px;
          margin-bottom: 15px;
        }

        p {
          font-size: 15px;
        }
      }
    }

    &-btn {
      button {
        font-size: 15px;
        padding: 10px 25px;
      }
    }
  }
}

@media screen and (max-width: 767.98px) {
  .features {
    &-title {
      h3 {
        margin-bottom: 5px;
      }

      p {
        font-size: 20px;
      }
    }

    &-interface {
      display: flex;
      flex-direction: column;
      padding: 30px 0;
    }

    .interface-title {
      font-size: 20px;
      margin-bottom: 15px;
    }

    .interface-curve {
      &:nth-child(3) {
        margin: 20px 0 20px 0;
      }

      .icon {
        width: 55px;
        height: 55px;
        margin-right: 30px;
      }
    }

    .interface-icon-text {
      font-size: 15px;
    }

    .tools {
      display: flex;
      flex-direction: column;

      &.reverse {
        display: flex;
        flex-direction: column;

        .tools-title {
          width: 100%;
          padding: 20px 0;
        }

        .tools-photo {
          width: 70%;
        }
      }

      &-title {
        width: 100%;
        padding: 20px;
        h5 {
          font-size: 25px;
          margin-bottom: 15px;
        }

        p {
          font-size: 15px;
        }
      }

      &-photo {
        width: 70%;
      }
    }

    &-btn {
      button {
        font-size: 15px;
        padding: 10px 25px;
      }
    }
  }
}

@media screen and (max-width: 575.98px) {
  .features {
    &-title {
      h3 {
        font-size: 25px;
        margin-bottom: 5px;
      }

      p {
        font-size: 15px;
      }
    }

    &-interface {
      display: flex;
      flex-direction: column;
      padding: 10px 0;
    }

    .interface-title {
      font-size: 20px;
      margin-bottom: 15px;
      text-align: center;
    }

    .interface-curve {
      &:nth-child(3) {
        margin: 20px 0 20px 0;
      }

      .icon {
        width: 55px;
        height: 55px;
        margin-right: 30px;
      }
    }

    .interface-icon-text {
      line-height: 1;
      font-size: 15px;
    }

    .tools {
      display: flex;
      flex-direction: column;

      &.reverse {
        display: flex;
        flex-direction: column;

        .tools-title {
          width: 100%;
          padding: 20px 0;
        }

        .tools-photo {
          width: 70%;
        }
      }

      &-title {
        width: 100%;
        padding: 20px;
        h5 {
          font-size: 25px;
          margin-bottom: 15px;
          text-align: center;
        }

        p {
          font-size: 15px;
          text-align: center;
        }
      }

      &-photo {
        width: 70%;
      }
    }

    &-btn {
      button {
        font-size: 15px;
        padding: 10px 25px;
      }
    }
  }
}
</style>
