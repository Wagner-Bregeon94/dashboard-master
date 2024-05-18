<template>
  <div class="content">
    <div class="container-fluid">
      <div class="row">
        <div class="col-12">
          <card class="strpied-tabled-with-hover"
            body-classes="table-full-width table-responsive">
            <template slot="header">
              <h4 class="card-title">Listagem de Produtos</h4>
            </template>

            <div>
              <h5>Roupas Masculinas</h5>
              <div>
                <label for="">Camisetas e Camisas</label>
                <select name="" id="">
                  <option value="">Camiseta</option>
                  <option value="">Camiseta Social</option>
                  <option value="">Camisa Polo</option>
                  <option value="">Camisa de Manga Longa</option>
                  <option value="">Regata</option>
                </select>
              </div>
              <div>
                <label for="">Calças e Bermudas</label>
                <select name="" id="">
                  <option value="">Calça Jeans</option>
                  <option value="">Calça Chino</option>
                  <option value="">Calça de Moletom</option>
                  <option value="">Bermuda</option>
                  <option value="">Calça Cargo</option>
                </select>
              </div>
              <div>
                <label for="">Roupas de Inverno</label>
                <select name="" id="">
                  <option value="">Jaqueta</option>
                  <option value="">Casaco</option>
                  <option value="">Moletom</option>
                  <option value="">Suéter</option>
                  <option value="">Blazer</option>
                </select>
              </div>
              <div>
                <label for="">Roupas Íntimas</label>
                <select name="" id="">
                  <option value="">Cueca</option>
                  <option value="">Meia</option>
                  <option value="">Pijama</option>
                  <option value="">Roupa de Dormir</option>
                  <option value="">Robe</option>
                </select>
              </div>
              <div>
                <label for="">Roupas Esportivas</label>
                <select name="" id="">
                  <option value="">Camiseta Esportiva</option>
                  <option value="">Shorts de Academia</option>
                  <option value="">Agasalho</option>
                  <option value="">Regata de Treino</option>
                  <option value="">Calça Esportiva</option>
                </select>
              </div>
              <div>
                <label for="">Acessórios</label>
                <select name="" id="">
                  <option value="">Boné</option>
                  <option value="">Chapéus</option>
                  <option value="">Cachecóis</option>
                  <option value="">Mochilas</option>
                  <option value="">Cintos</option>
                </select>
              </div>
            </div>
            
            <div>
              <h5>Roupas Femininas</h5>
              <div>
                <label for="">Vestidos</label>
                <select name="" id="">
                  <option value="">Vestido Casual</option>
                  <option value="">Vestido de Festa</option>
                  <option value="">Vestido Longo</option>
                  <option value="">Vestido Midi</option>
                  <option value="">Vestido Curto</option>
                </select>
              </div>
              <div>
                <label for="">Blusas e Camisas</label>
                <select name="" id="">
                  <option value="">Blusa de Manga Longa</option>
                  <option value="">Blusa de Manga Curta</option>
                  <option value="">Camisa Social</option>
                  <option value="">Camiseta</option>
                  <option value="">Regata</option>
                </select>
              </div>
              <div>
                <label for="">Calças e Saias</label>
                <select name="" id="">
                  <option value="">Calça Jeans</option>
                  <option value="">Calça Legging</option>
                  <option value="">Calça Social</option>
                  <option value="">Saia Longa</option>
                  <option value="">Saia Curta</option>
                </select>
              </div>
              <div>
                <label for="">Roupas de Inverno</label>
                <select name="" id="">
                  <option value="">Casaco</option>
                  <option value="">Jaqueta</option>
                  <option value="">Moletom</option>
                  <option value="">Cardigan</option>
                  <option value="">Suéter</option>
                </select>
              </div>
              <div>
                <label for="">Roupas Íntimas</label>
                <select name="" id="">
                  <option value="">Sutiã</option>
                  <option value="">Calcinha</option>
                  <option value="">Pijama</option>
                  <option value="">Robe</option>
                  <option value="">Lingerie</option>
                </select>
              </div>
              <div>
                <label for="">Acessórios</label>
                <select name="" id="">
                  <option value="">Bolsas</option>
                  <option value="">Chapéus</option>
                  <option value="">Cachecóis</option>
                  <option value="">Luvas</option>
                  <option value="">Cintos</option>
                </select>
              </div>
            </div>

            

           

          </card>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
  import LTable from 'src/components/Table.vue'
  import Card from 'src/components/Cards/Card.vue'
  const tableColumns = ['Id', 'Name', 'Salary', 'Country', 'City']
  const tableData = [{
    id: 1,
    name: 'Dakota Rice',
    salary: '$36.738',
    country: 'Niger',
    city: 'Oud-Turnhout'
  },
  {
    id: 2,
    name: 'Minerva Hooper',
    salary: '$23,789',
    country: 'Curaçao',
    city: 'Sinaai-Waas'
  },
  {
    id: 3,
    name: 'Sage Rodriguez',
    salary: '$56,142',
    country: 'Netherlands',
    city: 'Baileux'
  },
  {
    id: 4,
    name: 'Philip Chaney',
    salary: '$38,735',
    country: 'Korea, South',
    city: 'Overland Park'
  },
  {
    id: 5,
    name: 'Doris Greene',
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
