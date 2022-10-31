<script>
    import {setContext} from "svelte";
    import {writable} from "svelte/store";

    const testInformation = writable(1)

    const increment = () => {
        testInformation.update(prev => prev + 1)
    }

    setContext("test", {testInformation, increment})
</script>
<slot/>
