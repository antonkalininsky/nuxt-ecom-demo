<template>
  <div>
    <!-- header -->
    <div
      class="flex justify-between h-20 items-center px-10 text-sm font-bold border-b-2 w-100"
    >
      <div class="flex items-center">
        <div class="pr-12 cursor-pointer">
          <img src="/images/logo.svg" alt="gamepay" class="w-48" />
        </div>
        <button
          class="w-20 h-20 flex justify-center items-center border-x-2 hover:bg-red-500 hover:text-white transition"
        >
          <Icon name="material-symbols-light:menu" size="2rem" />
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
      <div
        class="flex gap-x-3 items-center hover:text-red-500 cursor-pointer leading-10 transition"
      >
        <Icon name="material-symbols-light:search" size="2rem" color="red" />
        <div>ПОИСК ИГР</div>
      </div>
      <div class="flex">
        <div
          class="cursor-pointer hover:bg-red-500 hover:text-white w-20 h-20 flex justify-center items-center transition"
        >
          <Icon name="ph:currency-rub-light" size="2rem" />
        </div>
        <div
          class="cursor-pointer hover:bg-red-500 hover:text-white w-20 h-20 flex justify-center items-center transition"
        >
          <Icon name="ion:cart-outline" size="2rem" />
        </div>
      </div>
    </div>
  </div>
</template>
