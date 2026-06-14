<template>
  <div class="dashboard">
    <div class="page-header">
      <h2 class="page-title">Dashboard</h2>
      <p class="page-subtitle">Engineering health at a glance</p>
    </div>
    <div class="cards">
      <div class="card">
        <h3 class="card-title">Health Summary</h3>
        <p class="card-body">No data yet. Connect a data source to get started.</p>
      </div>
      <div class="card">
        <h3 class="card-title">Throughput</h3>
        <p class="card-body">No data yet.</p>
      </div>
      <div class="card">
        <h3 class="card-title">Cycle Time</h3>
        <p class="card-body">No data yet.</p>
      </div>
      <div class="card">
        <h3 class="card-title">CI / Check Runs</h3>
        <p class="card-body">No data yet.</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.page-header {
  margin-bottom: 1.5rem;
}

.page-title {
  font-size: 1.5rem;
  font-weight: 700;
  color: #f1f5f9;
}

.page-subtitle {
  margin-top: 0.25rem;
  font-size: 0.875rem;
  color: #64748b;
}

.cards {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 1rem;
}

.card {
  background: #1e293b;
  border: 1px solid #334155;
  border-radius: 0.5rem;
  padding: 1.25rem;
}

.card-title {
  font-size: 0.875rem;
  font-weight: 600;
  color: #94a3b8;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  margin-bottom: 0.75rem;
}

.card-body {
  font-size: 0.875rem;
  color: #64748b;
}
</style>
