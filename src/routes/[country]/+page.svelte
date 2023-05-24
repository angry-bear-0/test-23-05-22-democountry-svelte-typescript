<script lang="ts">
  import { page } from "$app/stores";

  import Content from "../../components/Content.svelte";
  import GuideSection from "../../components/sections/GuideSection.svelte";

  import ShippingRateSection from "../../components/sections/ShippingRateSection.svelte";
  import TrackingSection from "../../components/sections/TrackingSection.svelte";
  import ShipmentsTypes from "../../components/sections/ShipmentsTypes.svelte";
  import RequiredDocSection from "../../components/sections/RequiredDocSection.svelte";
  import LimitItemsSection from "../../components/sections/LimitItemsSection.svelte";
  import DutiesAndTaxesSection from "../../components/sections/DutiesAndTaxesSection.svelte";
  import InsuranceSection from "../../components/sections/InsuranceSection.svelte";
  import FaqSection from "../../components/sections/FaqSection.svelte";

  let country = $page.params.country;
</script>

<div>
  <Content>
    <GuideSection country={country} />
    <ShippingRateSection country={country} />
    <TrackingSection />
    <ShipmentsTypes />
    <RequiredDocSection />
    <LimitItemsSection />
    <DutiesAndTaxesSection />
    <InsuranceSection />
    <FaqSection />
  </Content>
</div>
