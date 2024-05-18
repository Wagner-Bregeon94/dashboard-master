<template>
  <div class="content">
    <div class="container-fluid">
      <div class="row">
        <div class="col-12">
          <card class="strpied-tabled-with-hover"
            body-classes="table-full-width table-responsive">
            <template slot="header">
              <div class="row">
                <div class="col-8">
                  <h4 class="card-title">Listagem de Clientes</h4>
                </div>
                <div class="col-4">
                  <router-link :to="{name:'clients.create'}" class="btn btn-success btn-fill float-right">
                  Cadastrar Clientes
                  </router-link>
                </div>
              </div>
            </template>
            <l-table class="table-hover table-striped"
              :columns="table1.columns"
              :data="table1.data">
            </l-table>
          </card>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import LTable from 'src/components/Table.vue'
  import Card from 'src/components/Cards/Card.vue'
  const tableColumns = ['Id', 'Nome', 'Salary', 'Country', 'City']
  const tableData = [{
    id: 1,
    nome: 'Dakota Rice',
    salary: '$36.738',
    country: 'Niger',
    city: 'Oud-Turnhout'
  },
  {
    id: 2,
    nome: 'Minerva Hooper',
    salary: '$23,789',
    country: 'Curaçao',
    city: 'Sinaai-Waas'
  },
  {
    id: 3,
    nome: 'Sage Rodriguez',
    salary: '$56,142',
    country: 'Netherlands',
    city: 'Baileux'
  },
  {
    id: 4,
    nome: 'Philip Chaney',
    salary: '$38,735',
    country: 'Korea, South',
    city: 'Overland Park'
  },
  {
    id: 5,
    nome: 'Doris Greene',
    salary: '$63,542',
    country: 'Malawi',
    city: 'Feldkirchen in Kärnten'
  }]
  export default {
    components: {
      LTable,
      Card
    },
    data () {
      return {
        table1: {
          columns: [...tableColumns],
          data: [...tableData]
        },
        table2: {
          columns: [...tableColumns],
          data: [...tableData]
        }
      }
    }
  }
</script>
<style>
</style>
