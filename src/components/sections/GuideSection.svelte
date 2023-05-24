<script lang="ts">
  export let country = "";
  export let paragraphs = [
    "<p>Today's Netherlands was built by its global, seafaring people into a modern and industrial society. As a result of being one of the world's biggest traders today, the Netherlands is a top economic performer in Europe.</P>",
    "<p>And in the area of e-commerce, 14 million of the nation's 17 million people shop and purchase. In 2019, that will account for 14.5 billion USD of revenues, and growing at 7% per year. That can buy you a lot of gouda cheese!.</p>",
    "<p>Information on this page was found from <a>Netherlands Customs</a> and <a>European Union</a> Taxation , as well as from other Dutch government sources.</p>",
  ];
</script>

<div class="pt-[55px]">
  <h3 class="font-sec-title text-[30px] md:text-[34px]">
    Guide to Sending Parcel to the {country}
  </h3>
  {#each paragraphs as paragraph}
    <div>
      {@html paragraph}
    </div>
  {/each}
</div>
