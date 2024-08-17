<script setup>
import InputForm from "@/components/htmlTags/InputForm.vue";
import { reactive } from "vue";

let data = reactive({ email: "", password: "" });
</script>

<template>
    <section class="bg-gray-900">
        <div class="flex items-center justify-center min-h-screen py-8">
            <div class="w-1/3 bg-gray-800 border-gray-700 rounded-lg">
                <div class="p-6 space-y-4">
                    <h1 class="text-white font-bold text-xl">Tizimga Kirish</h1>
                    <form>
                        <div class="mb-5">
                            <InputForm
                                v-model="data.email"
                                labelName="Email"
                                inputType="email"
                                inputId="email"
                                inputName="email"
                                inputPlaceholder="name@gmail.com"
                            />
                        </div>
                        <div>
                            <InputForm
                                v-model="data.password"
                                labelName="Parol"
                                inputType="password"
                                inputId="password"
                                inputName="password"
                                inputPlaceholder="******"
                            />
                        </div>
                        <button
                            type="button"
                            class="text-white font-bold bg-blue-800 w-full mt-5 py-2 rounded hover:bg-blue-600 focus:ring-2"
                        >
                            Kirish
                        </button>
                        <div class="text-white">
                            {{ data }}
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped></style>
