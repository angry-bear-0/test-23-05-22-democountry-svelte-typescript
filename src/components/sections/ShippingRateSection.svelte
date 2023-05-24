<script lang="ts">
  import TruckIcon from "../icons/TruckIcon.svelte";
  import RightArrowIcon from "../icons/RightArrowIcon.svelte";
  import shippingImage from "$lib/images/sections/shipping-rates.jpg";
  export let country = "";

  let description = "Secureship provides safe and affordable shipping from Canada to the Netherlands. Whether you are an everyday shopper or a business, you can easily save up to 50% on your international shipping costs by way of accessing our group buying power.";
</script>

<div>
  <div class="flex items-center gap-[21px]">
    <TruckIcon />
    <h3 class="font-bold text-[24px] leading-[30px]">
      Cheap Shipping Rates to the {country}
    </h3>
  </div>
  <img
    src={shippingImage}
    alt="shipping rate"
    width="307"
    height="197"
  />
  <p>
    Easily compare the best and cheapest shipping options to {country} through a variety of carriers using Secureship
  </p>
  <p>
    {description}
  </p>
  <button class="flex items-center gap-[7px] mx-auto px-[23px] pt-[13px] pb-[15px] rounded-[10px] bg-[#FFA43C] text-white">
    Get an estimate 
    <RightArrowIcon/>
  </button>
</div>
