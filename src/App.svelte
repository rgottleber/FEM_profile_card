<script lang="ts">
  import Tailwindcss from "./Tailwindcss.svelte";
</script>

<Tailwindcss />

<main>
  <div class="card">
    <img src="/bg-pattern-card.svg" class="bg-card" />
    <div class="info">
      <div>
        <img src="image-victor.jpg" alt="victor" class="pic" />
      </div>
      <div class="name">Victor Crest <span class="age">26</span></div>
      <div class="city">London</div>
    </div>
    <div class="stats">
      <div>
        80K
        <div class="stat-type">Followers</div>
      </div>
      <div>
        803K
        <div class="stat-type">Likes</div>
      </div>
      <div>
        1.4K
        <div class="stat-type">Photos</div>
      </div>
    </div>
  </div>
  <img src="/bg-pattern-top.svg" class="bg-top" />
  <img src="/bg-pattern-bottom.svg" class="bg-bottom" />
</main>

<style>
  .stat-type {
    @apply font-thin;
    @apply text-gray-500;
    @apply text-sm;
  }
  .stats {
    @apply pt-4;
    @apply mt-72;
    @apply border-t-2;
    @apply grid;
    @apply grid-cols-3;
    @apply justify-items-center;
    @apply text-center;
    @apply font-black;
  }
  .city {
    @apply font-light;
    @apply text-gray-500;
    @apply text-sm;
    @apply pt-2;
  }
  .name {
    @apply pt-4;
    @apply font-bold;
  }
  .age {
    @apply font-light;
    @apply text-gray-500;
  }
  .pic {
    @apply rounded-full;
    @apply border-white;
    @apply border-4;
  }
  .info {
    @apply grid;
    @apply grid-cols-1;
    @apply justify-items-center;
    @apply z-10;
    @apply absolute;
    @apply w-full;
    @apply pt-24;
  }
  .card {
    @apply rounded-2xl;
    @apply bg-white;
    @apply h-96;
    @apply w-80;
    @apply fixed;
    @apply top-1/2;
    @apply left-1/2;
    @apply -mt-48;
    @apply -ml-40;
    @apply z-10;
    @apply shadow-md;
  }
  .bg-card {
    @apply w-full;
    @apply rounded-t-2xl;
    @apply absolute;
    @apply z-0;
  }
  .bg-top {
    @apply fixed;
    @apply -top-1/2;
    @apply -left-80;
    @apply h-full;
    @apply z-0;
  }
  .bg-bottom {
    @apply fixed;
    @apply -bottom-1/2;
    @apply -right-80;
    @apply h-full;
    /* @apply w-full; */
    @apply z-0;
  }
</style>
