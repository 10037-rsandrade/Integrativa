<template>
  <div class="user-list">
    <h2>Lista de Usuarios</h2>
    <ul>
      <li v-for="user in userList" :key="user.id">
        {{ user.name }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userList: [],
    };
  },
  mounted() {
    // Llamar a la función para obtener datos de la API simulada
    this.fetchUserList();
  },
  methods: {
    async fetchUserList() {
      try {
        // Realizar una solicitud HTTP a la API simulada
        const response = await fetch('https://jsonplaceholder.typicode.com/users');
        const data = await response.json();
        
        // Almacenar los datos de la API en la variable userList
        this.userList = data;
      } catch (error) {
        console.error('Error al obtener la lista de usuarios:', error);
      }
    },
  },
};
</script>

<style scoped>
.user-list {
  padding: 20px;
}
</style>
