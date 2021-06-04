<template>
  <div class="">
    <input type="text" placeholder="Add income like: Rent, 450 and press Enter" v-model="income" class="w-3/5 mr-2" v-on:keypress.enter="addIncomeItem(income)">
  </div>
</template>

<script>

import {INCOMES} from '../../constants/incomes.js'

export default {
  name: "AddIncome",
  data() {
    return {
      name: '',
      income: '',
      amount: 0,
      INCOMES: INCOMES
    }

  },
  methods: {
    incomeToArray() {
      this.income = this.income.split(',')
      this.name = this.income[0]
      this.amount = parseInt(this.income[1])
    },

    addIncomeItem() {
      this.incomeToArray()
      this.INCOMES.push({
        "name": this.name,
        "amount": this.amount
      })
      console.log(INCOMES)
      this.income = ''
    }
  }
}
</script>

<style scoped>

</style>
