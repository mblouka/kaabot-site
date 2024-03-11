<script>
  import "@fontsource-variable/inter"
  import "../app.pcss"

  import Icon from "@iconify/svelte"
</script>

<header class="mx-auto my-8 w-[65ch]">
  <div class="flex items-center gap-4 rounded-3xl border p-8">
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
      <a
        href="https://discord.com/oauth2/authorize?client_id=1215815540803895378&permissions=277025442880&scope=bot"
      >
        <button class="bg-green-600 font-semibold text-white">
          <Icon icon="fluent:add-12-filled" /> Add
        </button></a
      >
    </div>
  </div>
</header>

<main class="container prose prose-green mx-auto mb-8 rounded-3xl border p-8">
  <slot />
</main>
