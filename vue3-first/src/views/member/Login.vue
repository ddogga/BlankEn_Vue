<template>
  <div>
    <p class="tip">Double click on button in image container</p>
    <div class="cont">
      <div class="form sign-in">
        <h2 class="h2">Welcome back,</h2>
        <label class="label">
          <span>Email</span>
          <input class="input" type="email" />
        </label>
        <label class="label">
          <span>Password</span>
          <input class="input" type="password" />
        </label>
        <router-link class="nav-link active" aria-current="page" to="/">
          <p class="forgot-pass">Forgot password?</p>
        </router-link>
        <button type="button" class="submit button">Sign In</button>
        <button type="button" class="fb-btn button">
          Connect with <span>facebook</span>
        </button>

        <a
          href="https://dribbble.com/shots/3306190-Login-Registration-form"
          target="_blank"
          class="icon-link"
        >
          <img
            src="http://icons.iconarchive.com/icons/uiconstock/socialmedia/256/Dribbble-icon.png"
          />
        </a>
        <a
          href="https://twitter.com/NikolayTalanov"
          target="_blank"
          class="icon-link"
        >
          <img
            src="https://cdn1.iconfinder.com/data/icons/logotypes/32/twitter-128.png"
          />
        </a>
      </div>
      <div class="sub-cont">
        <div class="img">
          <div class="img__text m--up">
            <h2 class="h2">New here?</h2>
            <p>Sign up and discover great amount of new opportunities!</p>
          </div>
          <div class="img__text m--in">
            <h2 class="h2">One of us?</h2>
            <p>
              If you already has an account, just sign in. We've missed you!
            </p>
          </div>
          <div class="img__btn" @click="toggle">
            <span class="m--up">Sign Up</span>
            <span class="m--in">Sign In</span>
          </div>
        </div>
        <div class="form sign-up">
          <h2 class="h2">Time to feel like home,</h2>
          <label class="label">
            <span>Name</span>
            <input class="input" type="text" />
          </label>
          <label class="label">
            <span>Email</span>
            <input class="input" type="email" />
          </label>
          <label class="label">
            <span>Password</span>
            <input class="input" type="password" />
          </label>
          <button type="button" class="submit button">Sign Up</button>
          <button type="button" class="fb-btn button">
            Join with <span>facebook</span>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { change } from "@/assets/js/login.js";

export default {
  setup() {
    const toggle = () => {
      change();
    };

    return {
      toggle,
    };
  },
};
</script>

<style scoped></style>
