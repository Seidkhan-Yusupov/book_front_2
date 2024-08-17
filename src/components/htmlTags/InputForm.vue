<script setup>
defineProps({
    labelName: {
        type: String,
        default: "Email",
    },
    inputType: {
        type: String,
        default: "text",
    },
    inputName: {
        type: String,
        required: true,
    },
    inputId: {
        type: String,
    },
    inputPlaceholder: {
        type: String,
        default: "Write something here!",
    },
});
defineEmits(["update:modelValue"]);
</script>
<template>
    <label class="text-white font-bold" :for="inputId">{{ labelName }}</label>
    <input
        class="rounded border w-full bg-gray-700 border-gray-600 text-white p-2.5"
        :type="inputType"
        :name="inputName"
        :id="inputId"
        :placeholder="inputPlaceholder"
        @input="$emit('update:modelValue', $event.target.value)"
    />
</template>

<style lang="scss" scoped></style>
