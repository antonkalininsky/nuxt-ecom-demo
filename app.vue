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
        <MoreLink />
      </div>
      <div class="border-yellow-500 border-2">
        <SubHeaderNav title="Скидки" subtitle="от 40%" has-nav />
        <GameItemSmall />
        <GameItemSmall />
        <GameItemSmall />
        <GameItemSmall />
        <GameItemSmall />
        <GameItemSmall />
        <MoreLink />
        <SubHeaderNav title="Последние продажи" />
        <GameItemSmall />
        <GameItemSmall />
        <GameItemSmall />
      </div>
    </section>
  </div>
</template>
