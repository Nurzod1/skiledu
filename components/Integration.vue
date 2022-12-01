<template>
  <div class="integration">
    <div class="container">
      <div class="integration-wrapper">
        <div class="integration-part">
          <div class="intgeration-logos">
            <div class="google-t-logo">
              <div class="logo">
                <img src="@/assets/images/integer-1.svg" alt="" />
              </div>
              <div class="logo">
                <img src="@/assets/images/integer-2.svg" alt="" />
              </div>
              <div class="logo">
                <img src="@/assets/images/integer-3.svg" alt="" />
              </div>
              <div class="logo">
                <img src="@/assets/images/integer-4.svg" alt="" />
              </div>
            </div>
          </div>
          <div class="integration-items">
            <p class="pre-title">INTEGRATIONS</p>
            <div class="main-title">
              <h3>
                200+ educational tools and platform <span>integrations</span>
              </h3>
              <p>
                Schoology has every tool your classroom needs and comes
                pre-integrated with more than 200+ tools, student information
                systems (SIS), and education platforms.
              </p>
            </div>
            <div class="integration-btn">
              <button>See All Integrations</button>
            </div>
          </div>
        </div>

        <div class="testimonial">
          <div class="testimonials-items">
            <p class="pre-title">TESTIMONIAL</p>
            <div class="main-title">
              <h3>What They Say?</h3>
              <p>
                Skilline has got more than 100k positive ratings from our users
                around the world.
              </p>
              <p>
                Some of the students and teachers were greatly helped by the
                Skilline.
              </p>
              <p>Are you too? Please give your assessment</p>
            </div>
            <div class="testimonial-btn">
              <button>
                <span>Write your assessment</span>
                <div class="arrow-icon">
                  <svg
                    width="24"
                    height="24"
                    xmlns="http://www.w3.org/2000/svg"
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                  >
                    <path
                      d="M21.883 12l-7.527 6.235.644.765 9-7.521-9-7.479-.645.764 7.529 6.236h-21.884v1h21.883z"
                    />
                  </svg>
                </div>
              </button>
            </div>
          </div>
          <div class="testimonials-photo">
            <div class="photo-wrapper">
              <img src="@/assets/images/test-woman.png" alt="" />
              <div class="photo-arrow">
                <img src="@/assets/images/arrow-right.svg" alt="" />
              </div>
            </div>
            <div class="review">
              <p class="review-text">
                "Thank you so much for your help. It's exactly what I've been
                looking for. You won't regret it. It really saves me time and
                effort. Skilline is exactly what our business has been lacking."
              </p>
              <div class="rated">
                <h6>Gloria Rose</h6>
                <div class="stars-text">
                  <div class="stars">
                    <svg
                      v-for="item in 5"
                      :key="item"
                      xmlns="http://www.w3.org/2000/svg"
                      width="24"
                      height="24"
                      viewBox="0 0 24 24"
                    >
                      <path
                        d="M12 .587l3.668 7.568 8.332 1.151-6.064 5.828 1.48 8.279-7.416-3.967-7.417 3.967 1.481-8.279-6.064-5.828 8.332-1.151z"
                      />
                    </svg>
                  </div>
                  <p class="text">12 reviews at Yelp</p>
                </div>
              </div>
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
.integration {
  padding: 100px 0;

  &-wrapper {
    display: flex;
    flex-direction: column;
  }

  .integration-part {
    display: flex;
    align-items: center;
    justify-content: center;
  }

  &-logos {
    display: flex;
    flex-direction: column;
    width: 50%;
  }

  .google-t-logo {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
  }

  .logo {
    width: 160px;
    height: 160px;

    img {
      width: 100%;
      height: 100%;
    }
  }

  &-items {
    display: flex;
    flex-direction: column;
    width: 50%;
    padding: 50px;
    position: relative;
  }

  .pre-title {
    font-family: Nun;
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 27px;
    letter-spacing: 0.2em;
    color: #525596;
    transform: translateX(20%);
    position: relative;

    &::before {
      background: #525596;
      content: "";
      width: 80px;
      height: 1px;
      top: 50%;
      left: -20%;
      position: absolute;
    }
  }

  .main-title {
    margin: 33px 0 40px 0;

    h3 {
      font-family: Nun;
      font-weight: bold;
      font-size: 36px;
      line-height: 160%;
      color: #2f327d;
      margin-bottom: 30px;

      span {
        color: #f48c06;
      }
    }

    p {
      font-family: Nun;
      font-weight: normal;
      font-size: 24px;
      color: #696984;

      &:nth-child(3) {
        margin: 26px 0 46px 0;
      }
    }
  }

  &-btn {
    margin-top: 43px;

    button {
      color: #f48c06;
      background: transparent;
      font-family: Nun;
      font-weight: normal;
      font-size: 22px;
      line-height: 180%;
      padding: 20px 42px;
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

  .testimonial {
    display: flex;
    padding-top: 50px;
  }

  .testimonials-items {
    width: 50%;
    padding: 50px;
  }

  .testimonial-btn {
    button {
      font-weight: normal;
      font-size: 22px;
      padding: 22px 100px 22px 38px;
      color: #f48c06;
      background: transparent;
      display: flex;
      align-items: center;
      border: none;
      border: 1px solid #f48c06;
      border-radius: 40px;
      transition: 0.2s cubic-bezier(0.9, 0.85, 0.175, 1);
      position: relative;
      cursor: pointer;

      &:hover {
        color: #ffffff;
        background: #f48c06;

        svg {
          fill: #ffffff;
        }
      }
    }
  }

  .arrow-icon {
    padding: 27px;
    border: 1px solid #f48c06;
    border-radius: 50%;
    display: flex;
    align-items: center;
    position: absolute;
    top: 0;
    right: 0%;
    bottom: 0;

    svg {
      fill: #f48c06;
    }
  }

  .testimonials-photo {
    position: relative;
    width: 50%;

    .photo-wrapper {
      display: flex;
      position: relative;
      width: 80%;
      max-width: 600px;

      img {
        width: 100%;
        height: 100%;
        border-radius: 20px;
        overflow: hidden;
      }
    }

    .photo-arrow {
      position: absolute;
      top: 50%;
      right: 0;
      display: flex;
      align-items: center;
      width: 60px;
      height: 60px;
      padding: 20px;
      background: #ffffff;
      border-radius: 50%;
      box-shadow: 0px 4px 60px rgba(41, 44, 124, 0.15);
      transform: translate(50%, -50%);
    }
  }

  .review {
    position: absolute;
    left: 0;
    bottom: 0;
    width: 100%;
    padding: 20px 30px 20px 35px;
    background: #ffffff;
    border-radius: 20px;
    border-left: 15px solid #f67766;
    box-shadow: 2px 4px 60px rgba(41, 44, 124, 0.1);
    transform: translate(10%, 30%);
    z-index: 2;

    &-text {
      border-left: 1px solid #2f327d;
      font-family: Nun;
      font-weight: normal;
      font-size: 20px;
      color: #5f5f7e;
      margin-bottom: 43px;
      margin-left: 30px;
    }
  }

  .rated {
    display: flex;
    align-items: center;
    justify-content: space-between;

    h6 {
      font-family: Nun;
      font-weight: 600;
      font-size: 22px;
      color: #5f5f7e;
    }
  }

  .stars {
    display: flex;
    align-items: center;
    justify-content: center;

    svg {
      fill: #fba333;
    }
  }

  .text {
    font-family: Nun;
    font-weight: 600;
    font-size: 18px;
    color: #80819a;
  }
}

@media screen and (max-width: 1199.98px) {
  .integration {
    .pre-title {
      font-size: 15px;

      &::before {
        width: 70px;
      }
    }

    .main-title {
      h3 {
        font-size: 30px;
      }

      p {
        font-size: 20px;

        &:nth-child(3) {
          margin: 20px 0 40px 0;
        }
      }
    }

    &-btn {
      button {
        font-size: 20px;
        padding: 15px 30px;
      }
    }

    .testimonial-btn {
      button {
        font-size: 20px;
      }
    }

    .review {
      padding: 20px 30px 20px 20px;

      &-text {
        margin-bottom: 35px;
        padding-left: 15px;
      }
    }

    .rated {
      h6 {
        font-size: 20px;
      }
    }
  }
}

@media screen and (max-width: 991.98px) {
  .integration {
    .pre-title {
      font-size: 12px;

      &::before {
        width: 40px;
      }
    }

    .main-title {
      h3 {
        font-size: 22px;
        margin-bottom: 15px;
      }

      p {
        font-size: 15px;

        &:nth-child(3) {
          margin: 20px 0 40px 0;
        }
      }
    }

    &-btn {
      button {
        font-size: 15px;
        padding: 13px 30px;
      }
    }

    .testimonials-items {
      padding: 25px;
    }

    .testimonial-btn {
      button {
        font-size: 15px;
        white-space: nowrap;
        padding: 20px 90px 20px 30px;
      }

      .arrow-icon {
        padding: 17px;
      }
    }

    .review {
      padding: 20px 30px 20px 20px;

      &-text {
        font-size: 15px;
        margin-bottom: 25px;
        padding-left: 15px;
      }
    }

    .rated {
      h6 {
        font-size: 15px;
      }

      .stars {
        width: 80px;
      }

      .text {
        font-size: 13px;
      }
    }
  }
}

@media screen and (max-width: 767.98px) {
  .integration {
    .pre-title {
      font-size: 12px;

      &::before {
        position: absolute;
        top: 45%;
        width: 75px;
      }
    }

    &-part {
      display: flex;
      flex-direction: column;
    }

    &-items {
      padding: 20px;
      width: 100%;
    }

    .main-title {
      margin: 33px 0 25px 0;

      h3 {
        font-size: 22px;
        margin-bottom: 15px;
      }

      p {
        font-size: 15px;

        &:nth-child(3) {
          margin: 20px 0 40px 0;
        }
      }
    }

    &-btn {
      margin-top: 20px;

      button {
        font-size: 15px;
        padding: 13px 30px;
      }
    }

    .testimonial {
      display: flex;
      flex-direction: column;
      padding-top: 20px;
    }

    .testimonials-items {
      padding: 20px;
      width: 100%;
    }

    .testimonial-btn {
      button {
        font-size: 15px;
        white-space: nowrap;
        padding: 20px 90px 20px 30px;
      }

      .arrow-icon {
        padding: 17px;
      }
    }

    .testimonials-photo {
      width: 70%;
      .photo-wrapper {
        width: 100%;
      }
    }

    .review {
      padding: 15px 10px 15px 10px;
      transform: translate(0%, 50%);

      &-text {
        font-size: 12px;
        margin-bottom: 10px;
        padding-left: 10px;
      }
    }

    .rated {
      h6 {
        font-size: 12px;
      }

      .stars {
        width: 60px;
      }

      .text {
        font-size: 12px;
      }
    }
  }
}

@media screen and (max-width: 575.98px) {
  .integration {
    .pre-title {
      font-size: 12px;
      transform: translateX(0%);
      text-align: center;
      &::before {
        display: none;
      }
    }

    .logo {
      width: 130px;
      height: 130px;
    }

    &-part {
      display: flex;
      flex-direction: column;
    }

    &-items {
      padding: 20px;
      width: 100%;
    }

    .main-title {
      margin: 10px 0 20px 0;

      h3 {
        font-size: 22px;
        margin-bottom: 15px;
        text-align: center;
      }

      p {
        font-size: 15px;
        text-align: center;

        &:nth-child(3) {
          margin: 15px 0 15px 0;
        }
      }
    }

    &-btn {
      display: flex;
      justify-content: center;
      margin-top: 20px;

      button {
        font-size: 15px;
        padding: 13px 30px;
      }
    }

    .testimonial {
      display: flex;
      flex-direction: column;
      padding-top: 20px;
    }

    .testimonials-items {
      padding: 20px;
      width: 100%;
    }

    .testimonial-btn {
      display: flex;
      justify-content: center;

      button {
        font-size: 15px;
        white-space: nowrap;
        padding: 20px 90px 20px 30px;
      }

      .arrow-icon {
        padding: 17px;
      }
    }

    .testimonials-photo {
      display: flex;
      flex-direction: column;
      align-items: center;
      width: 100%;

      .photo-wrapper {
        width: 90%;
      }
    }

    .review {
      position: static;
      padding: 10px 10px 10px 10px;
      transform: translate(0%, 0%);

      &-text {
        font-size: 12px;
        margin-bottom: 5px;
        padding-left: 10px;
        margin-left: 5px;
      }
    }

    .rated {
      h6 {
        font-size: 12px;
      }

      .stars {
        width: 60px;
      }

      .text {
        font-size: 12px;
      }
    }
  }
}
</style>
