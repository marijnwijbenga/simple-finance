<template>
  <li v-for="(income, index) in INCOMES.slice().reverse()"
      class="bg-green-300 text-green-800 font-semibold rounded mb-2 p-4">
    <div class="flex flex-row flex-nowrap">
      <div class="w-8/12">
        {{ income.name }}
      </div>
      <div class="w-4/12 text-right pr-4">
        {{ income.amount}}
      </div>
    </div>
  </li>
</template>

<script>
import {INCOMES} from '../../constants/incomes.js'

export default {
  name: "IncomeItem",
  data() {
    return {

      INCOMES: INCOMES

    }

  }
}
</script>

<style scoped>

</style>
