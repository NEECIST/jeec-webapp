<template>
  <div class="who-are-we-comp">
    <component-title title="Who are we?" subtitle="JEECIST" />

    <div class="who-are-we-text">
      <span v-html="text"></span>
    </div>

    <div class="activities-container">
      <div class="activity-flex">
        <p
          class="activity"
          v-for="activity in activities"
          v-bind:key="activity.name"
        >
          <b>{{ activity.name }}</b>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "who-are-we",
  data() {
    return {
      text:
        "A group of <b>IST</b> students, whose main purpose is to organize an event with the intention of closing the gap between the business world and university life.<p>Participation is free of charge and open to a strong student community with over 11000 aspiring engineers.</p><p>Activities available at JEEC:</p>",
    };
  },
  props: {
    activities: Array,
  },
  methods: {
    openNav() {
      document.getElementById("mySidenav").style.width = "250px";
    },

    closeNav() {
      document.getElementById("mySidenav").style.width = "0";
    },
  },
};
</script>

<style>
.who-are-we-comp {
  width: 100%;
  background-color: #ffffff;
  padding-top: 10px;
  padding-bottom: 15px;
  text-align: center;
}

.who-are-we-text {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 75%;
  font-family: "Lato";
  margin-top: 20px;
  font-size: 25px;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  line-height: 35px;
  letter-spacing: normal;
  color: #505050;
  display: inline-block;
}

.activities-container {
  text-align: center;
  width: 100%;
  margin-top: -10px;
}

.activity-flex {
  display: flex;
  display: -webkit-box; /* OLD - iOS 6-, Safari 3.1-6 */
  display: -moz-box; /* OLD - Firefox 19- (buggy but mostly works) */
  display: -ms-flexbox; /* TWEENER - IE 10 */
  display: -webkit-flex; /* NEW - Chrome */
  justify-content: space-around;
  flex-wrap: wrap;
  align-content: center;
  justify-content: center;
  align-items: center;
}

.activity {
  font-family: "Lato";
  margin-top: 20px;
  font-size: 25px;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  line-height: 35px;
  letter-spacing: normal;
  color: #505050;
  margin: 25px;
  padding: 10px;
  background-color: rgb(223, 230, 245);
  border-radius: 15px;
}

/* On screens that are 992px wide or less*/
@media only screen and (max-width: 992px) {
  .who-are-we-text {
    width: 90%;
  }
}

/* On screens that are 600px wide*/
@media only screen and (max-width: 600px) {
  .who-are-we-text {
    width: 95%;
    font-size: 16px;
    line-height: 25px;
  }

  .activity {
    font-size: 16px;
    line-height: 25px;
    margin: 10px;
    padding: 5px;
    border-radius: 8px;
  }

  .div-title {
    font-size: 30px;
  }
}
</style>
