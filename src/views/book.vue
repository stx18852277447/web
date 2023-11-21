<template>
    <div>
        <label for="bookCategory">选择类别:</label>
        <select id="bookCategory" v-model="selectedCategory">
            <option v-for="category in bookCategories" :key="category" :value="category">
                {{ category }}
            </option>
        </select>
        <p>选的是: {{ selectedCategory }}</p>
    </div>
</template>
  
<script>
export default {
    data() {
        return {
            selectedCategory: null,
            bookCategories: ["计算机", "文学", "历史"],
        };
    },
};
</script>

<style scoped></style>
  