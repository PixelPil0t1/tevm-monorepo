<script lang="ts">
import { QueryClient, QueryClientProvider } from '@tanstack/svelte-query'
import '../app.css'

const queryClient = new QueryClient()
</script>

<QueryClientProvider client={queryClient}>
    <slot />
</QueryClientProvider>