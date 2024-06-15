<template>
  <div>
    <NavMain />
    <PanelCarousel />
    <!-- items -->
    <section class="grid grid-cols-[2fr_1fr] gap-x-5 w-4/5 mx-auto py-5">
      <div class="border-pink-500 border-2">
        <div class="mb-5 border-b-2">
          <SideNavItem> Новинки </SideNavItem>
          <SideNavItem is-active> Лидеры продаж </SideNavItem>
          <SideNavItem> Ожидаемые </SideNavItem>
        </div>
        <GameItem />
        <GameItem />
        <GameItem />
        <GameItem />
        <GameItem />
        <a
          class="w-full text-center py-10 hover:text-red-500 transition flex justify-center items-center gap-x-1"
          href=""
        >
          <div class="text-xs font-semibold">Посмотреть все игры</div>
          <Icon class="text-red-500 text-sm" name="mingcute:down-fill" />
        </a>
      </div>
      <div class="border-yellow-500 border-2"></div>
    </section>
  </div>
</template>
