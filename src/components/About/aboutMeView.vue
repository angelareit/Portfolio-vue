<script>
export default {
  setup() {
    return {
      bios: [
        {
          id: 1,
          bio:
            'Hi, There!',
        },
        {
          id: 2,
          bio:
            `My name is Angela Tabafunda, a full stack developer based in Toronto, Ontario.\nI love making things work and making it work well - Delivered to provide good experien ce. Overall, I like to make software that everyone would like to use.`,
        },
      ],
    };
  },
};
</script>

<template>
  <div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
    <!-- About profile image -->
    <div class="w-full sm:w-1/4 mb-7 sm:mb-0">
      <img
        src="https://img.atlasobscura.com/pKkD1QdauLKYjLtwlMBTlgssVTnUZqmF2Ey2UvcQuOI/rt:fit/w:1280/q:81/sm:1/scp:1/ar:1/aHR0cHM6Ly9hdGxh/cy1kZXYuczMuYW1h/em9uYXdzLmNvbS91/cGxvYWRzL2Fzc2V0/cy8xMzUzNTYxNzRi/Y2Y0N2Q2YzlfR2V0/dHlJbWFnZXMtNTIw/NDQyODE4LmpwZw.jpg"
        class="rounded-xl w-96" alt="" />
    </div>

    <!-- About details -->
    <div class="w-full sm:w-3/4 text-left">
      <p v-for="bio in bios" :key="bio.id"
        class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg">
        {{ bio.bio }}
      </p>
    </div>
  </div>
</template>