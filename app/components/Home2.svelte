<page>
    <actionBar title="Home"/>
    <stackLayout>
        <label class="info">
            <formattedString>
                <span text=" {$testInformation}"/>
            </formattedString>
        </label>
        <button text="Increment" on:tap="{increment}"/>
        <button text="Navigate to next page" on:tap="{nextPage}"/>
    </stackLayout>
</page>

<script lang="ts">
    import {getContext} from "svelte";
    import {navigate} from "svelte-native";
    import Home from "./Home.svelte";

    const {testInformation, increment} = getContext("test")

    const nextPage = () => {
        navigate({
            page: Home,
            clearHistory: true,
            animated: false
        })
    }

</script>

<style>
    .info {
        font-size: 20;
        horizontal-align: center;
        vertical-align: center;
    }
</style>
