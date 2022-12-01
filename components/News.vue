<template>
  <div class="news">
    <div class="container">
      <div class="news-wrapper">
        <div class="news-title">
          <h3>Lastest News and Resources</h3>
          <p>
            See the developments that have occurred to Skillines in the world
          </p>
        </div>
        <div class="news-second-wrapper">
          <div class="main-news full">
            <div class="main-photo">
              <img src="@/assets/images/news-1.png" alt="" />
            </div>
            <p class="main-text">News</p>
            <div class="main-info">
              <h6>
                Class adds $30 million to its balance sheet for a Zoom-friendly
                edtech solution
              </h6>
              <p>
                Class, launched less than a year ago by Blackboard co-founder
                Michael Chasen, integrates exclusively...
              </p>
              <a href="#">Read more</a>
            </div>
          </div>
          <div class="news-category full">
            <div class="category-info">
              <div class="category-photo">
                <img src="@/assets/images/news-2.png" alt="" />
                <p>Press Realase</p>
              </div>
              <div class="about-category">
                <h6>
                  Class Technologies Inc. Closes $30 Million Series A Financing
                  to Meet High Demand
                </h6>
                <p>
                  Class Technologies Inc., the company that created Class,...
                </p>
              </div>
            </div>
            <div class="category-info">
              <div class="category-photo">
                <img src="@/assets/images/news-3.png" alt="" />
                <p>Press Realase</p>
              </div>
              <div class="about-category">
                <h6>
                  Class Technologies Inc. Closes $30 Million Series A Financing
                  to Meet High Demand
                </h6>
                <p>
                  Class Technologies Inc., the company that created Class,...
                </p>
              </div>
            </div>
            <div class="category-info">
              <div class="category-photo">
                <img src="@/assets/images/news-4.png" alt="" />
                <p>Press Realase</p>
              </div>
              <div class="about-category">
                <h6>
                  Class Technologies Inc. Closes $30 Million Series A Financing
                  to Meet High Demand
                </h6>
                <p>
                  Class Technologies Inc., the company that created Class,...
                </p>
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
.news {
  padding: 100px 0;

  &-title {
    display: flex;
    flex-direction: column;
    align-items: center;

    h3 {
      font-family: Nun;
      font-weight: bold;
      font-size: 36px;
      color: #2f327d;
    }

    p {
      font-family: Nun;
      font-weight: normal;
      font-size: 24px;
      text-align: center;
      color: #696984;
    }
  }

  &-second-wrapper {
    display: flex;
    gap: 50px;
    margin-top: 50px;
  }

  .main {
    &-photo {
      margin-bottom: 40px;

      img {
        width: 100%;
        height: auto;
      }
    }

    &-text {
      width: fit-content;
      font-weight: 500;
      font-size: 20px;
      color: #252641;
      background: #f4c467;
      border: 1px solid #f4c467;
      border-radius: 40px;
      padding: 2px 35px;
    }

    &-info {
      margin-top: 20px;

      h6 {
        font-weight: 500;
        font-size: 26px;
        color: #252641;
      }

      p {
        font-weight: normal;
        font-size: 20px;
        color: #696984;
        margin: 20px 0 28px 0;
      }

      a {
        font-weight: normal;
        font-size: 20px;
        text-decoration-line: underline;
        color: #696984;
      }
    }
  }

  .news {
    &-category {
      width: 80%;
    }
  }

  .category {
    &-info {
      display: flex;
      align-items: flex-start;

      &:not(:last-child) {
        margin-bottom: 50px;
      }
    }

    &-photo {
      position: relative;
      display: flex;
      width: 200px;

      img {
        width: 100%;
        height: 100%;
        object-fit: cover;
      }

      p {
        font-size: 15px;
        color: #252641;
        background: #f4c467;
        border: 1px solid #f4c467;
        border-radius: 40px;
        padding: 4px 12px;
        position: absolute;
        right: 6px;
        bottom: 8px;
      }
    }
  }

  .about-category {
    flex: 1;
    margin-left: 40px;

    h6 {
      font-weight: 500;
      font-size: 22px;
      color: #252641;
      margin-bottom: 20px;
    }

    p {
      font-weight: normal;
      font-size: 20px;
      color: #696984;
    }
  }
}

@media screen and (max-width: 1199.98px) {
  .news {
    &-title {
      h3 {
        font-size: 30px;
      }

      p {
        font-size: 20px;
      }
    }

    .main {
      &-photo {
        margin-bottom: 30px;
      }

      &-info {
        h6 {
          font-size: 23px;
        }

        p {
          font-size: 17px;
        }
      }
    }

    .about-category {
      h6 {
        font-size: 20px;
      }

      p {
        font-size: 17px;
      }
    }
  }
}

@media screen and (max-width: 991.98px) {
  .news {
    &-title {
      h3 {
        font-size: 30px;
      }

      p {
        font-size: 20px;
      }
    }

    .news-second-wrapper {
      display: grid;

      &.full {
        display: grid;
        grid-column: 1 / span 4;
      }
    }

    .main {
      &-photo {
        margin-bottom: 30px;
      }

      &-info {
        h6 {
          font-size: 23px;
        }

        p {
          font-size: 17px;
        }
      }
    }

    .about-category {
      h6 {
        font-size: 20px;
      }

      p {
        font-size: 17px;
      }
    }
  }
}

@media screen and (max-width: 767.98px) {
  .news {
    &-title {
      h3 {
        font-size: 30px;
      }

      p {
        font-size: 20px;
      }
    }

    .news-second-wrapper {
      display: grid;

      &.full {
        display: grid;
        grid-column: 1 / span 4;
      }
    }

    .main {
      &-photo {
        margin-bottom: 30px;
      }

      &-info {
        h6 {
          font-size: 23px;
        }

        p {
          font-size: 17px;
        }
      }
    }

    &-category-part {
      width: 100%;
    }

    .category-info {
      margin-bottom: 30px;
    }

    .about-category {
      h6 {
        font-size: 20px;
      }

      p {
        font-size: 17px;
      }
    }
  }
}

@media screen and (max-width: 575.98px) {
  .news {
    padding: 50px 0;

    &-title {
      h3 {
        text-align: center;
        font-size: 20px;
      }

      p {
        text-align: center;
        font-size: 15px;
      }
    }

    .news-second-wrapper {
      display: grid;

      &.full {
        display: grid;
        grid-column: 1 / span 4;
      }
    }

    .main {
      &-photo {
        margin-bottom: 25px;
      }

      &-text {
        font-size: 15px;
      }

      &-info {
        h6 {
          font-size: 20px;
        }

        p {
          font-size: 15px;
          margin: 10px 0 15px 0;
        }

        a {
          font-size: 15px;
        }
      }
    }

    &-category-part {
      width: 100%;
    }

    &-category.full {
      width: 100%;
    }

    .category-info {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-bottom: 25px;

      &:not(:last-child) {
        margin-bottom: 35px;
      }
    }

    .category-photo {
      width: 100%;
      margin-bottom: 15px;
    }

    .about-category {
      margin-left: 0;

      h6 {
        font-size: 15px;
      }

      p {
        font-size: 12px;
      }
    }
  }
}
</style>
