<template>
  <div class="flex flex-col items-center">
    <!-- header -->
    <div
      class="flex justify-between h-20 items-center px-10 text-sm font-bold border-b-2"
    >
      <div class="flex items-center">
        <div class="pr-6">
          <img src="/images/logo.svg" alt="gamepay" class="w-48" />
        </div>
        <button class="w-10 h-10 flex justify-center items-center">
          <MdiIcon icon="mdiMenu" :size="'100'" view-box="0 0 24 24" />
        </button>
        <nav>
          <ul class="flex px-6">
            <li
              class="px-6 hover:text-red-500 cursor-pointer leading-10 transition"
            >
              КАТАЛОГ ПРОДУКЦИИ
            </li>
            <li
              class="px-6 hover:text-red-500 cursor-pointer leading-10 transition"
            >
              ПОДДЕРЖКА
            </li>
            <li
              class="px-6 hover:text-red-500 cursor-pointer leading-10 transition"
            >
              МОИ ПОКУПКИ
            </li>
          </ul>
        </nav>
      </div>
      <div>ПОИСК ИГР</div>
      <div class="flex">
        <div>money</div>
        <div>cart</div>
      </div>
    </div>
  </div>
</template>
