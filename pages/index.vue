<template>
  <div>
    <Banner />
    <div class="flex justify-center py-12">
      <div class="text-center space-y-3">
        <h1 class="uppercase text-4xl font-bold tracking-wide">
          Gifts for the fam
        </h1>
        <h3>
          Everything to give all those Energy Matchers, Rule Breakers, and more.
        </h3>
        <div class="flex justify-center space-x-2">
          <button
            class="text-white bg-black px-8 py-2 rounded-full tracking-wider"
          >
            Shop
          </button>
          <button
            class="text-white bg-black px-8 py-2 rounded-full tracking-wider"
          >
            Gift Guide
          </button>
        </div>
      </div>
    </div>
    <ItemCard :items="items" />
    <slot></slot>
  </div>
</template>

<script setup>
let items = [
  {
    id: 32,
    name: 'Nike',
    options: [
      {
        id: 356,
        price: '$11,000',
        imgPath:
          'https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/bac14469-a46c-4d81-afde-4637f920d210/blazer-low-77-womens-shoes-01lVDq.png',
      },
      {
        id: 8932,
        price: '$700',
        imgPath:
          'https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/1f3c4476-8c68-4e0f-af4d-ebc3a0528e29/blazer-low-77-se-womens-shoes-01lVDq.png',
      },
      {
        id: 8932,
        price: '$1900',
        imgPath:
          'https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/5804adcd-94a4-41f6-b29b-509a07e86d47/blazer-low-77-womens-shoes-01lVDq.png',
      },
    ],
  },
  {
    id: 32,
    name: 'Pants',
    options: [
      {
        id: 3672,
        price: '$4500',
        imgPath:
          'https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/c2faf415-f8c8-4da8-83b1-9eaaeaedb231/sportswear-club-fleece-womens-holiday-sweatshirt-SBXMSx.png',
      },
      {
        id: 9832,
        price: '$1700',
        imgPath:
          'https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/9b4e0da1-d6b1-4464-a349-e6be22e1d934/sportswear-club-fleece-womens-holiday-sweatshirt-SBXMSx.png',
      },
      {
        id: 239832,
        price: '$1700',
        imgPath:
          'https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/122c0b81-46ec-42c7-b408-b7a8b849b076/sportswear-club-fleece-womens-holiday-sweatshirt-SBXMSx.png',
      },
    ],
  },
  {
    id: 98082,
    name: 'Jordan Essentials',
    options: [
      {
        id: 3672,

        price: '$90',
        imgPath:
          'https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/16429793-1f3e-491a-987f-c34f0d971f1d/sportswear-phoenix-fleece-womens-oversized-crewneck-sweatshirt-kdpTnT.png',
      },
      {
        price: '$300',
        imgPath:
          'https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/47b7d7ed-17a3-4c23-809a-e35586773dab/sportswear-phoenix-fleece-womens-oversized-crewneck-sweatshirt-kdpTnT.png',
      },
      {
        price: '$200',
        imgPath:
          'https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/c6438884-3739-42d4-b6e7-ec4137593491/sportswear-phoenix-fleece-womens-oversized-crewneck-sweatshirt-kdpTnT.png',
      },
      {
        price: '$65',
        imgPath:
          'https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/4ad41d3d-cffb-4751-a07a-e5b94ab4781f/sportswear-phoenix-fleece-womens-oversized-crewneck-sweatshirt-kdpTnT.png',
      },
    ],
  },
];
</script>