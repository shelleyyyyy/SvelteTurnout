<script>
    export let placeHolder;
    export let label;

    let value = "";

    const HandleChange = () => {
        console.log(value);
    }

</script>

<section>
    <div class="m-5">
        <label for="first_name" class="block mb-2 text-sm font-medium">{label}</label>
        <input on:change={() => HandleChange()} bind:value={value} type="text" id="first_name" class="border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:border-gray-600 dark:placeholder-gray-400 dark:focus:ring-blue-500 dark:focus:border-blue-500" placeholder={placeHolder} required>
    </div>
</section>