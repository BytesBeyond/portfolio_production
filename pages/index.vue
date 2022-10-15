<template>
  <div>
    {{ filtersList }}
  </div>
</template>

<script>
import {useFiltersStore} from '~/store/filters'
import {defineComponent} from "vue/types/v3-define-component";

export default defineComponent({
  setup() {
    const filtersStore = useFiltersStore()
    const filtersList = filtersStore.filtersList

    return {filtersList}
  },
})
</script>
