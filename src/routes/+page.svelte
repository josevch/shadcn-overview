
	
<script lang="ts">
    import * as Accordion from "$lib/components/ui/accordion";
    import { Button } from "$lib/components/ui/button";
    import { Switch } from "$lib/components/ui/switch";
    import { Calendar } from "$lib/components/ui/calendar";
  import { today, getLocalTimeZone } from "@internationalized/date";

  let value = today(getLocalTimeZone());
  </script>
  <div class="mx-auto w-96  ">
    <Accordion.Root >
        <Accordion.Item value="item-1">
          <Accordion.Trigger>Is it accessible?</Accordion.Trigger>
          <Accordion.Content>
            Yes. It adheres to the WAI-ARIA design pattern.
          </Accordion.Content>
        </Accordion.Item>
      </Accordion.Root>
      
      
        
      <Button variant="outline">Button</Button>
    
      <Switch />
    
      <Calendar bind:value class="border rounded-md shadow" />
  </div>
