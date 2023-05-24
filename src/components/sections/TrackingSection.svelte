<script lang="ts">
  import PointerIcon from "../icons/PointerIcon.svelte";
  import WarningIcon from "../icons/WarningIcon.svelte";
  import timeLineImage from '$lib/images/sections/timeline.png';
  export let country = "";

</script>

<div>
  <div class="flex items-center gap-[21px]">
    <PointerIcon />
    <h3 class="font-bold text-[24px] leading-[30px]">
      Easy Tracking Information
    </h3>
  </div>
  <p class="font-medium text-[18px] leading-[28px]">
    Shipments through Secureship come with full, easy to read tracking
    information to {country}
  </p>
  <img src={timeLineImage} alt="timelineimage"/>
  <div class="px-[28px] pt-[33px] pb-[39px] border-[3px] border-[#CB0F51] rounded-[11px] ">
    <div class="flex items-center gap-[9px] font-bold text-[16px] leading-[28px] text-[#CB0F51]">
      <WarningIcon/>
      Disclaimer
    </div>
    <p class="font-normal text-[16px] leading-[28px] text-[#36134A] ">
      While we have made every effort to ensure that the information on this page is accurate, Customs laws and procedures change regularly so it is important to consult a licensed broker in {country} before shipping any goods.
    </p>
  </div>
</div>
