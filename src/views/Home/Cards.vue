<template>
  <div class="flex justify-center w-full mt-2" @click="hello()">
    <div class="max-w-sm rounded overflow-hidden shadow-lg">
      <img class="w-40 mx-auto" src="../../assets/images/git_squash.png" alt="Plants vs Zombie's Squasher (Chayote)">
      <div class="px-6 py-4">
        <div class="font-bold text-xl mb-2 text-center">Squashing Git Commits</div>
        <p class="text-gray-700 text-base">
          Squash irrelevant commits in order to keep a cleaner commit history.
        </p>
      </div>
      <div class="px-6 py-4">
        <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#git</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  setup () {
    function hello () {
      alert('ping')
    }

    return { hello }
  }
}
</script>

<style>

</style>
