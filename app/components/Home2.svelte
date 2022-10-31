<page>
    <actionBar title="Home" />
    <stackLayout>
        <label class="info">
            <formattedString>
                <span text=" {$testInformation}" />
            </formattedString>
        </label>
        <button text="Increment" on:tap="{increment}" />
        <button text="Navigate to next page" on:tap="{increment}" />
    </stackLayout>
</page>

<script lang="ts">
    import {getContext} from "svelte";

    let message: string = "Blank Svelte Native App"
    const {testInformation, increment} = getContext("test")

</script>

<style>
    .info .fas {
        color: #3A53FF;
    }

    .info {
        font-size: 20;
        horizontal-align: center;
        vertical-align: center;
    }
</style>
