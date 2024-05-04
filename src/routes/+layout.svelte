<script>
  import "@fontsource-variable/inter"
  import "../app.pcss"

  import Icon from "@iconify/svelte"
</script>

<header class="mx-auto my-8 w-[65ch]">
  <div class="flex items-center gap-4 rounded-3xl border-2 border-zinc-800 p-8">
    <div class="h-[50px] min-h-[50px] w-[50px] min-w-[50px]">
      <img src="./logo.svg" alt="Kaaba" />
    </div>
    <div class="max-w-xs">
      <div class="text-xl font-bold">Kaab'ot</div>
      <div class="text-xs opacity-80">
        Bring the boundless light of Islam to your server with Kaab'ot, the Islamic Discord bot
      </div>
    </div>
    <div class="ml-auto flex gap-2">
      <a href="https://add.kaabot.org">
        <button>
          <Icon icon="fluent:add-12-filled" /> Add
        </button></a
      >
    </div>
  </div>
</header>

<div class="container mx-auto w-[65ch] rounded-3xl border-2 border-zinc-800">
  <nav class="flex">
    <a href="/"><Icon icon="heroicons:home" class="text-4xl" />Home</a>
    <a href="/commands"><Icon icon="heroicons:code-bracket" class="text-4xl" />Commands</a>
    <a href="/community"><Icon icon="heroicons:radio" class="text-4xl" />Community</a>
    <a href="/about"><Icon icon="heroicons:information-circle" class="text-4xl" />About</a>
  </nav>
  <main class="prose prose-green prose-invert p-8">
    <slot />
  </main>
</div>

<style lang="postcss">
  nav a {
    @apply flex flex-1 flex-col items-center gap-1 border-b-2 border-r-2 border-zinc-800 py-3 text-xs text-zinc-600 last:border-r-0 hover:border-b-green-500 hover:text-green-500;
  }
</style>
