<template>
  <q-page>
    <div class="q-pa-md">
      <q-table
        title="Treats"
        :rows="rows"
        :columns="columns"
        row-key="name"
      />
    </div>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
  data () {
    return {
      columns: [
        {
          name: 'title',
          field: 'title',
          required: true,
          label: 'Titulo',
          align: 'left',
          sortable: true
        }
      ],
      rows: [
        {
          title: 'Anotação 1'
        },
        {
          title: 'Anotação 2'
        }
      ]
    }
  }
}
</script>
