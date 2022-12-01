<template>
  <div class="cloud">
    <div class="container">
      <div class="cloud-wrapper">
        <div class="cloud-title">
          <h3>All-In-One <span>Cloud Software.</span></h3>
          <p>
            Skilline is one powerful online software suite that combines all the
            tools needed to run a successful school or office.
          </p>
        </div>
        <div class="cloud-infos-wrapper">
          <div class="cloud-block">
            <div class="block-img">
              <img src="@/assets/images/contracts.svg" alt="" />
            </div>
            <h5 class="block-title">Online Billing, Invoicing, & Contracts</h5>
            <p class="block-subtitle">
              Simple and secure control of your organization’s financial and
              legal transactions. Send customized invoices and contracts
            </p>
          </div>
          <div class="cloud-block">
            <div class="block-img">
              <img src="@/assets/images/calendar.svg" alt="" />
            </div>
            <div class="block-title">
              <h5>Easy Scheduling & Attendance Tracking</h5>
            </div>
            <div class="block-subtitle">
              <p>
                Schedule and reserve classrooms at one campus or multiple
                campuses. Keep detailed records of student attendance
              </p>
            </div>
          </div>
          <div class="cloud-block">
            <div class="block-img">
              <img src="@/assets/images/customer.svg" alt="" />
            </div>
            <div class="block-title">
              <h5>Customer Tracking</h5>
            </div>
            <div class="block-subtitle">
              <p>
                Automate and track emails to individuals or groups. Skilline’s
                built-in system helps organize your organization
              </p>
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
.cloud {
  padding: 50px 0;

  &-wrapper {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }

  &-title {
    h3 {
      font-style: normal;
      font-weight: bold;
      font-size: 36px;
      text-align: center;
      color: #2f327d;
      margin-bottom: 20px;

      span {
        color: #f48c06;
      }
    }

    p {
      font-style: normal;
      font-weight: normal;
      font-size: 24px;
      text-align: center;
      color: #696984;
    }
  }

  &-infos-wrapper {
    display: flex;
    gap: 50px;
  }

  &-block {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 50px 40px;
    margin-top: 100px;
    background: #ffffff;
    box-shadow: 0px 10px 60px rgba(38, 45, 118, 0.08);
    border-radius: 20px;

    .block-img {
      transform: translateY(-100%);
      width: 48px;
      height: 48px;
      padding: 10px;
      background: #5b72ee;
      box-shadow: 0px 10px 40px rgba(54, 61, 136, 0.06);
      border-radius: 50%;

      img {
        width: 100%;
        height: 100%;
        object-fit: contain;
      }
    }

    .block-title {
      margin-bottom: 25px;
      font-weight: 500;
      font-size: 30px;
      text-align: center;
      color: #2f327d;
    }

    .block-subtitle {
      font-weight: normal;
      font-size: 20px;
      text-align: center;
      color: #696984;
    }
  }
}

@media screen and (max-width: 1199.98px) {
  .cloud {
    &-block {
      padding: 40px 30px;

      .block-title {
        font-size: 25px;
      }
    }
  }
}

@media screen and (max-width: 991.98px) {
  .cloud {
    &-title {
      h3 {
        font-size: 30px;
        margin-bottom: 10px;
      }

      p {
        font-size: 20px;
      }
    }

    &-block {
      padding: 30px 20px;
      margin-top: 60px;

      .block-title {
        font-size: 20px;
        margin-bottom: 15px;
      }

      .block-subtitle {
        font-size: 15px;
      }
    }
  }
}

@media screen and (max-width: 767.98px) {
  .cloud {
    padding: 30px 0;

    &-title {
      h3 {
        font-size: 25px;
        margin-bottom: 10px;
      }

      p {
        font-size: 15px;
      }
    }

    &-block {
      padding: 25px 10px;
      margin-top: 40px;

      .block-img {
        width: 40px;
        height: 40px;
      }

      .block-title {
        font-size: 15px;
        margin-bottom: 10px;
      }

      .block-subtitle {
        font-size: 12px;
      }
    }
  }
}

@media screen and (max-width: 575.98px) {
  .cloud {
    padding: 30px 0;

    &-title {
      h3 {
        font-size: 20px;
        margin-bottom: 10px;
      }

      p {
        font-size: 12px;
      }
    }

    &-infos-wrapper {
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    &-block {
      max-width: 350px;
      padding: 20px 12px;
      margin-top: 30px;

      .block-img {
        width: 40px;
        height: 40px;
      }

      .block-title {
        font-size: 14px;
        margin-bottom: 10px;
      }

      .block-subtitle {
        font-size: 10px;
      }
    }
  }
}
</style>
