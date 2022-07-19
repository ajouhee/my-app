<script lang="ts">
import { Button } from "@src/components/button";

const textNumbers: string[] = ['1', '2', '3', '4', '5', '6', '7', '8', '9','0','.'];

const textSusik: string[] = ['%', 'CE', 'C','del'];

const textSusik2: string[] = ['/', 'X','-','+']

const textSum: string[] = ['='];


</script>

<div class="frame1">
    {#each textSusik as text}
    <Button {text} color="dark-grey" onClick={(value) => alert(value)} />
    {/each}
</div>

<div class="frame2">
    {#each textSusik2 as text}
    <Button {text} color="dark-grey" onClick={(value) => alert(value)} />
    {/each}
</div>

<div class="frame">
    {#each textNumbers as text}
        <Button {text} color="orange" onClick={(value) => alert(value)} />
    {/each}

    {#each textSum as text}
        <Button {text} color="grey" onClick={(value) => alert(value)} />
    {/each}
</div>

