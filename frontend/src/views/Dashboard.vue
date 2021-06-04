<template>
  <page-wrapper>
    <heading-wrapper>
      <balance-total></balance-total>
    </heading-wrapper>
    <section-wrapper>
      <income-list>
        <add-income></add-income>
        <income-item></income-item>
      </income-list>
      <expenditure-list>
        <expenditure-item></expenditure-item>
      </expenditure-list>
    </section-wrapper>
    <footer-wrapper>
    </footer-wrapper>
  </page-wrapper>
</template>

<script>
import PageWrapper from '../components/layout/PageWrapper.vue';
import HeadingWrapper from '../components/layout/HeadingWrapper.vue';
import SectionWrapper from '../components/layout/SectionWrapper.vue';
import FooterWrapper from '../components/layout/FooterWrapper.vue';
import BalanceTotal from '../components/globals/BalanceTotal.vue';
import IncomeList from '../components/incomes/IncomeList.vue';
import AddIncome from '../components/incomes/AddIncome.vue';
import IncomeItem from '../components/incomes/IncomeItem.vue';
import ExpenditureList from '../components/expenditures/ExpenditureList.vue';
import ExpenditureItem from '../components/expenditures/ExpenditureItem.vue';

export default {
name: "Dashboard",
  components: {FooterWrapper, SectionWrapper, HeadingWrapper, PageWrapper, BalanceTotal, IncomeList, IncomeItem, ExpenditureList, ExpenditureItem, AddIncome}
}
</script>

<style scoped>

</style>
