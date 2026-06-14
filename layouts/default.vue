<template>
  <div class="layout">
    <aside class="sidebar">
      <div class="sidebar-header">
        <h1 class="sidebar-title">Clawd Metrics</h1>
      </div>
      <nav class="sidebar-nav">
        <NuxtLink to="/" class="nav-link" exact-active-class="active">
          Dashboard
        </NuxtLink>
        <NuxtLink to="/metrics" class="nav-link" exact-active-class="active">
          Metrics
        </NuxtLink>
      </nav>
    </aside>
    <main class="main">
      <slot />
    </main>
  </div>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  background: #0f172a;
  color: #e2e8f0;
}

.layout {
  display: flex;
  min-height: 100vh;
}

.sidebar {
  width: 240px;
  background: #1e293b;
  border-right: 1px solid #334155;
  display: flex;
  flex-direction: column;
}

.sidebar-header {
  padding: 1.25rem;
  border-bottom: 1px solid #334155;
}

.sidebar-title {
  font-size: 1rem;
  font-weight: 600;
  color: #f1f5f9;
  letter-spacing: 0.025em;
}

.sidebar-nav {
  padding: 0.75rem;
  display: flex;
  flex-direction: column;
  gap: 0.25rem;
}

.nav-link {
  display: block;
  padding: 0.5rem 0.75rem;
  border-radius: 0.375rem;
  color: #94a3b8;
  text-decoration: none;
  font-size: 0.875rem;
  transition: background 0.15s, color 0.15s;
}

.nav-link:hover {
  background: #334155;
  color: #e2e8f0;
}

.nav-link.active {
  background: #1d4ed8;
  color: #fff;
}

.main {
  flex: 1;
  padding: 1.5rem;
  overflow-y: auto;
}
</style>
