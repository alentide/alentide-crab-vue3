<template>
  <div class="text-white flex flex-col text-[14px]">
    <div class="bg-[#002D74] flex justify-between">
      <div class="flex items-center h-14">
        <div class="px-3 inline-flex justify-center items-center text-white h-full hover:bg-[#00235B] cursor-pointer"
          v-for="item in 3">
          <div>图</div>
          <div class="text-sm ml-1">文字{{item}}</div>
        </div>
      </div>
      <div class="inline-flex items-center text-white">
        <div class="cursor-pointer hover:bg-[#00235B] h-full px-4 items-center inline-flex">登录</div>
      </div>
    </div>
    <div class="px-3 bg-[#002051] flex-1">
      <div class="space-x-2 py-3 test">
        <button class="bg-[#00CFE3] hover:bg-[rgba(#00CFE3,0.5)] px-5 py-[1px] ">打卡</button>
        <button class="bg-red-500 disabled:bg-blue hover:bg-red-700 px-5 py-[1px] ">打卡打卡打卡</button>
      </div>

      <table class="border-collapse border bg-[#002051] border-[#0B3373] w-full">
        <thead class="bg-[#1B50A8]">
          <tr class="border-b-1">
            <th ></th>
            <th >State</th>
            <th>City</th>
          </tr>
        </thead>
        <tbody>
          <tr class="text-center">
            <td class="border border-[#0B3373]">[]</td>
            <td class="border border-[#0B3373]">Indiana</td>
            <td class="border border-[#0B3373]">Indianapolis</td>
          </tr>
          <tr>
             <td class="border border-[#0B3373]">[]</td>
            <td class="border border-[#0B3373]">Ohio</td>
            <td class="border border-[#0B3373]">Columbus</td>
          </tr>
          <tr>
             <td class="border border-[#0B3373]">[]</td>
            <td class="border border-[#0B3373]">Michigan</td>
            <td class="border border-[#0B3373]">Detroit</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>


<script setup lang="ts">
import { onMounted, ref } from 'vue';

</script>

<style scoped>
.test {
  font-size: 14px;
}
</style>