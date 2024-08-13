<template>
  <div class="h-11 bg-sky-600 align-center text-center text-white pt-2">
    <span>A Webflow template for SaaS products. </span>
    <span class="text-gray-600">See all templates ></span>
  </div>
  <div class="mx-60">
    <Cap />

    <UnderTheCap />

    <div class="text-center mt-20">
      <h1 class="text-xl">Trusted by 50,000+ companies</h1>
      <div class="flex justify-center space-x-5 mt-5">
        <img src="/firefox.svg" alt="" />
        <img src="/nowintech.svg" alt="" />
        <img src="/optimer.svg" alt="" />
        <img src="/carder.svg" alt="" />
      </div>
    </div>

    <CardList />
  </div>
  <div class="mt-20 bg-slate-200">
    <div class="mx-60 py-20">
      <h2 class="text-5xl">We will take care of everything,</h2>
      <h2 class="text-5xl">so you can get back to relaxing.</h2>

      <div class="flex justify-between mt-20">
        <div>
          <TitleArrow :item="item" v-for="item in arrow" :key="item" />
        </div>

        <img src="/tele.svg" alt="" />
      </div>
    </div>
  </div>
  <About />
  <SetForget />
  <Tasks />
  <Blog />
  <div class="mx-60">
    <div class="bg-sky-100 p-10 my-20 space-y-5">
      <div class="space-y-5 w-2/6">
        <h2 class="text-4xl">Get started with Whirl</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.
        </p>
        <button class="bg-sky-600 text-white px-5 py-2">Book a demo</button>
      </div>
      <div class="flex items-center">
        <span class="w-52 relative">
          <img src="/check.svg" alt="" class="stroke-black" />
          <p class="absolute left-5 -top-1 text-inherit">Understand your options</p> </span
        ><span class="w-52 relative">
          <img src="/check.svg" alt="" class="stroke-black" />
          <p class="absolute left-5 -top-1 text-inherit">Understand your options</p>
        </span>
      </div>
    </div>
  </div>
  <div class="mx-60 py-20">
    <div class="flex justify-between py-10">
      <div>
        <div class="x-5 flex items-center">
          <img src="/logo.svg" alt="" class="h-10" />
          <img src="/whirl.svg" alt="" class="h-6 ml-2" />
        </div>
        <p class="mt-4">Built by <q class="text-sky-600">Nikolai Bain</q></p>
        <p>Powered by <q class="text-sky-600">Webflow</q></p>
      </div>
      <div class="flex space-x-10">
        <div>
          <p class="pb-5"><b>Info</b></p>
          <p>Features</p>
          <p>Pricing</p>
          <p>Blog</p>
          <p>Support</p>
          <p>Terms & Conditions</p>
          <p>Privacy Policy</p>
        </div>
        <div>
          <p class="pb-5"><b>Info</b></p>
          <p>Style Guide</p>
          <p>Licenses</p>
          <p>Instructions</p>
          <p>Changelog</p>
          <p>Password</p>
          <p>404</p>
        </div>
        <div>
          <p class="pb-5"><b>Newsletter</b></p>
          <p class="w-48">Sign up for the latest news, company insights, and Whirl updates.</p>
          <div class="relative">
            <input
              type="text"
              placeholder="Your email"
              class="mt-4 appearance-none w-full border-b border-slate-300 py-2 px-3 text-gray-700 focus:outline-none focus:shadow-outline"
            />
            <img
              src="/arrow.svg "
              alt=""
              class="absolute right-0 top-7 transition hover:translate-x-1"
            />
          </div>
        </div>
      </div>
    </div>
    <div class="border-t border-slate-300 flex justify-between py-10">
      <div>
        © 2022 Whirl. All Rights Reserved. Illustrations by <q class="text-sky-600">Streamline</q>
      </div>
      <div class="flex space-x-5">
        <img src="/twiter.svg" alt="" />
        <img src="/linkedin.svg" alt="" />
        <img src="/facebook.svg" alt="" />
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

import Cap from './components/Cap.vue'
import UnderTheCap from './components/UnderTheCap.vue'
import CardList from './components/CardList.vue'
import TitleArrow from './components/TitleArrow.vue'
import Tasks from './components/Tasks.vue'
import About from './components/About.vue'
import SetForget from './components/SetForget.vue'
import Blog from './components/Blog.vue'
const arrow = ref([
  {
    img: '/anti.svg',
    title: 'Anti-loss technology',
    text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.'
  },
  {
    img: '/smile.svg',
    title: 'Exchange easily',
    text: ''
  },
  {
    img: '/mail.svg',
    title: 'Anti-loss technology',
    text: ''
  },
  {
    img: '/thunder.svg',
    title: 'Exchange easily',
    text: ''
  }
])
</script>

<style lang="scss" scoped></style>
