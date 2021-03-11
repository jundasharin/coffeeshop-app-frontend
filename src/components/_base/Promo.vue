<template>
  <div class="Promo pt-5 text-center">
    <h3>Promo Today</h3>
    <p>Coupons Will be updated every weeks<br />Check them out!</p>
    <div class="button-promo">
      <b-row
        class="coupon mt-4 mx-auto"
        v-for="(item, index) in promo"
        :key="index"
      >
        <b-button>
          <b-row>
            <b-col cols="4">
              <b-img></b-img>
            </b-col>
            <b-col cols="8">
              <h5 class="text-left">{{ item.promo_name }}</h5>
              <p class="text-left">{{ item.promo_desc }}</p>
            </b-col>
          </b-row>
        </b-button>
      </b-row>
    </div>
    <div>
      <b-button class="apply-bttn mt-4">
        <h5 class="m-0 py-2">
          Apply Coupons
        </h5>
      </b-button>
    </div>
    <div class="tc text-left pl-5">
      <p><b>Terms & Condition</b></p>
      <p>1. You can only apply 1 coupon per day</p>
      <p>2. It only for dine in</p>
      <p>3. Buy 1 get 1 only for new user</p>
      <p>4. Should make member card to apply coupon</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Promo",
  data() {
    return {
      promo: [
        {
          promo_id: 2,
          promo_name: "Happy Sunday",
          promo_desc: "Get one of our Coffee if you theacher"
        },
        {
          promo_id: 3,
          promo_name: "Happy Satnight",
          promo_desc: "Get one of our Coffee every Sunday"
        },
        {
          promo_id: 4,
          promo_name: "Happy Sunday",
          promo_desc: "Get one of our Coffee if you theacher"
        },
        {
          promo_id: 5,
          promo_name: "Happy Satnight",
          promo_desc: "Get one of our Coffee every Sunday"
        }
      ]
    }
  }
}
</script>

<style>
/* .Promo {
  background-color: violet;
  height: 150px;
} */

.button-promo {
  position: relative;
  height: 250px;
  overflow-y: auto;
}

.coupon {
  width: 270px;
}

.apply-bttn {
  width: 270px;
  background-color: #6a4029 !important;
  color: white;
}

.tc {
  margin-top: 50px;
  padding-bottom: 50px;
}

.tc p {
  margin: 0px;
}
</style>
