<script setup>
import { defineProps } from 'vue';

defineProps({
    title: {
        type: String,
        default: 'Vaggelis Chaniotakis',
    },
    subtitle: {
        type: String,
        default: 'MSc. Software Engineer',
    }
});
</script>

<template>
    <section class="bg-blue-700 py-20 mb-4">
      <div
        class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col items-center"
      >
        <div class="text-center">
          <h1
            class="text-4xl font-extrabold text-white sm:text-5xl md:text-6xl">
            {{ title }}
          </h1>
          <p class="my-4 text-xl text-white">
            {{ subtitle }}
          </p>
        </div>
      </div>
    </section>
    <section class="py-6">
      <div class="container-xl lg:container m-auto">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-4 p-4 rounded-lg">
          <Card>
            <h2 class="text-2xl font-bold">Connect with me on Linkedin</h2>
            <br/>
            <a
            href="https://www.linkedin.com/in/vaggelis-chaniotakis-b0b894120/"
            target="_blank"
            rel="noopener noreferrer"
            class="inline-block bg-blue-500 text-white rounded-lg px-4 py-2 hover:bg-blue-600"
            >
            LinkedIn
            </a>
        </Card>
        <Card bg="bg-blue-100">
          <h2 class="text-2xl font-bold">Send me an email</h2>
          <br/>
            <a
            href="mailto:chaniotakisv@gmail.com"
            target="_blank"
            rel="noopener noreferrer"
            class="inline-block bg-red-500 text-white rounded-lg px-4 py-2 hover:bg-red-600"
            >
            Email
            </a>
          </Card>
        </div>
      </div>
    </section>
</template>