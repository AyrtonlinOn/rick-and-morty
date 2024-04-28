<template>
  <div class="container my-5">
    <div class="row justify-content-center">
      <div class="col-md-8">
        <h1 class="text-center mb-4">Sobre o Aluno</h1>
        <div class="card p-4">
          <div class="mb-4">
            <h2>Aluno</h2>
            <p><strong>Nome:</strong> Ayrton Lima Oliveira</p>
            <p><strong>RA:</strong> 1957939</p>
            <p><strong>Curso:</strong> Análise e Desenvolvimento de Sistemas</p>
          </div>
          <div class="mb-4">
            <h2>Universidade</h2>
            <p><strong>Nome:</strong> Unimar (Universidade de Marília)</p>
            <p><strong>Cidade:</strong> Marília</p>
            <p><strong>Estado:</strong> São Paulo</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SobrePage'
}
</script>

<style>
.card {
  border: 1px solid #ddd;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1)
}
</style>

