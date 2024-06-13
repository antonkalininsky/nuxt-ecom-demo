<template>
  <div>
    <NavMain />
    <section
      class="w-full bg-slate-800 h-[550px] flex flex-col justify-center items-center py-5 gap-y-5"
    >
      <!-- panels -->
      <div class="w-4/5 h-full grid grid-cols-3 grid-rows-2">
        <PanelItem class="row-span-2 col-span-2" is-main />
        <PanelItem />
        <PanelItem />
      </div>
      <!-- panels nav -->
      <div class="flex justify-between items-center w-2/3 text-white">
        <Icon name="mingcute:left-line" size="2rem" />
        <div class="flex gap-x-2">
          <div class="size-2 bg-white rounded-full"></div>
          <div class="size-2 bg-white rounded-full"></div>
          <div class="size-2 bg-white rounded-full"></div>
          <div
            class="size-2 bg-white rounded-full"
            :class="{ 'bg-blue-500': true }"
          ></div>
        </div>
        <Icon name="mingcute:right-line" size="2rem" />
      </div>
    </section>
  </div>
</template>
