<script>
    import {setContext} from "svelte";
    import {writable} from "svelte/store";
    const testInformation = writable("1234")

    setContext("test", testInformation)
</script>
<slot/>
