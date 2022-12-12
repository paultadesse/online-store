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
    <!-- membership -->
    <div class="relative px-10 py-4">
      <img
        alt="Nike. Just Do It"
        class=""
        src="https://static.nike.com/a/images/f_auto/dpr_1.0,cs_srgb/w_1778,c_limit/5e4a0ef7-a2c9-483a-8e5b-45d8277db19d/nike-just-do-it.jpg"
      />
      <div class="absolute top-0.5 xl:top-1/2 text-white px-7 xl:space-y-3">
        <p class="uppercase xl:text-6xl font-bold">become a member</p>
        <p class="tracking-wider">Sign up for free. Join the community.</p>
        <button class="bg-white text-black px-6 py-2 rounded-full">Join Us</button>
      </div>
    </div>
    <!-- <slot></slot> -->
  </div>
</template>

<script setup>
let items = [
  [
    {
      id: 32,
      name: "Nike",
      options: [
        {
          id: 356,
          price: "$11,000",
          imgPath:
            "https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/bac14469-a46c-4d81-afde-4637f920d210/blazer-low-77-womens-shoes-01lVDq.png",
        },
        {
          id: 8932,
          price: "$700",
          imgPath:
            "https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/1f3c4476-8c68-4e0f-af4d-ebc3a0528e29/blazer-low-77-se-womens-shoes-01lVDq.png",
        },
        {
          id: 8932,
          price: "$1900",
          imgPath:
            "https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/5804adcd-94a4-41f6-b29b-509a07e86d47/blazer-low-77-womens-shoes-01lVDq.png",
        },
      ],
    },
  ],
  [
    {
      id: 32,
      name: "Pants",
      options: [
        {
          id: 3672,
          price: "$4500",
          imgPath:
            "https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/c2faf415-f8c8-4da8-83b1-9eaaeaedb231/sportswear-club-fleece-womens-holiday-sweatshirt-SBXMSx.png",
        },
        {
          id: 9832,
          price: "$1700",
          imgPath:
            "https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/9b4e0da1-d6b1-4464-a349-e6be22e1d934/sportswear-club-fleece-womens-holiday-sweatshirt-SBXMSx.png",
        },
        {
          id: 239832,
          price: "$1700",
          imgPath:
            "https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/122c0b81-46ec-42c7-b408-b7a8b849b076/sportswear-club-fleece-womens-holiday-sweatshirt-SBXMSx.png",
        },
      ],
    },
  ],

  [
    {
      id: 98082,
      name: "Jordan Essentials",
      options: [
        {
          id: 3672,

          price: "$90",
          imgPath:
            "https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/16429793-1f3e-491a-987f-c34f0d971f1d/sportswear-phoenix-fleece-womens-oversized-crewneck-sweatshirt-kdpTnT.png",
        },
        {
          price: "$300",
          imgPath:
            "https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/47b7d7ed-17a3-4c23-809a-e35586773dab/sportswear-phoenix-fleece-womens-oversized-crewneck-sweatshirt-kdpTnT.png",
        },
        {
          price: "$200",
          imgPath:
            "https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/c6438884-3739-42d4-b6e7-ec4137593491/sportswear-phoenix-fleece-womens-oversized-crewneck-sweatshirt-kdpTnT.png",
        },
        {
          price: "$65",
          imgPath:
            "https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/4ad41d3d-cffb-4751-a07a-e5b94ab4781f/sportswear-phoenix-fleece-womens-oversized-crewneck-sweatshirt-kdpTnT.png",
        },
      ],
    },
  ],

  [
    {
      id: 35987,
      name: "Nike Air icon Fleece",
      options: [
        {
          price: "$65",
          imgPath:
            "https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/bf37d1df-1cc5-49ae-93c5-6e226df51676/air-icon-fleece-big-kids-crew-neck-sweatshirt-13Mctx.png",
        },
        {
          price: "$65",
          imgPath:
            "https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/91c3eb31-07c6-4481-b74e-7d29aba41c21/air-icon-fleece-big-kids-crew-neck-sweatshirt-13Mctx.png",
        },
      ],
    },
  ],
  [
    {
      id: 987642,
      name: "Nike Solo Swoosh",
      options: [
        {
          price: "$90",
          imgPath:
            "https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/e23374b1-9d01-49fa-9e19-9f26479765c3/solo-swoosh-mens-fleece-pants-90h6N2.png",
        },
        {
          price: "$75",
          imgPath:
            "https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/a791ce8b-e317-4407-b0d3-c6419cd3c9e3/solo-swoosh-mens-fleece-pants-90h6N2.png",
        },
        {
          price: "$85",
          imgPath:
            "https://static.nike.com/a/images/c_limit,w_592,f_auto/t_product_v1/64fe31b6-3517-4b9f-a83c-ddd664e19e64/solo-swoosh-mens-fleece-pants-90h6N2.png",
        },
      ],
    },
  ],
  [
    {
      id: 567123,
      name: "Air Jordan 3 Retro",
      options: [
        {
          price: "$200",
          imgPath:
            "https://static.nike.com/a/images/q_auto:eco/t_product_v1/f_auto/dpr_1.0/h_595,c_limit/3ae019aa-92be-4c35-85a4-0e6acca796c3/air-jordan-3-retro-womens-shoes-XTx5gw.png",
        },
      ],
    },
  ],
];
</script>
