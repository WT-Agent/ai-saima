<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****7700 设计了销售战区双十一冲刺对赌 PK 方案"
  },
  {
    "text": "用户 189****3311 生成了 3 个研发小组并行攻坚赛马规则"
  },
  {
    "text": "用户 131****9922 完成了全国代理商月度回款实时榜单激励"
  },
  {
    "text": "用户 156****4455 生成了跨部门转介绍裂变奖金池分配细则"
  },
  {
    "text": "用户 177****8890 取得了防止赛马恶性抢单的风控 SOP 规则"
  }
]);
</script>
