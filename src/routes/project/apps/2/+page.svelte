<script>

</script>


<main>
    <!-- svelte-ignore missing-declaration -->
    <div class="table" items={items}>
        <div class="title">
            <div class="item"></div>
            <div class="item"></div>
        </div>
        <div class="main" let:item={item}>
            <div class="item date">{item.date}</div>
            <div class="item name">{item.name}</div>
        </div>
    </div>
</main>


<style>


</style>