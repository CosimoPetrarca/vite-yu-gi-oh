<script>
export default {
    name: 'Search'
}
</script>

<template>
    <div class="container">
        <form>
            <div class="row justify-content-start">
            
            <div class="col-2 col-sm-auto">
                <label for="search-status" class="form-label d-none">Select Status</label>
                <select class="form-select" id="search-status">
                    <option selected>Select Status</option>
                    <option value="1">One</option>
                    <option value="2">Two</option>
                    <option value="3">Three</option>
                </select>
            </div>
            
        </div>
        </form>
    </div>
</template>

<style lang="scss" scoped>
select{
    margin: 30px 0;
}
</style>