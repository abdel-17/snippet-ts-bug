<!-- everything works when the script tag is at the top -->
<!-- <script lang="ts"></script> -->

{#snippet foo({ props }: { props?: Record<string, unknown> })}{/snippet}

<!-- this won't error if you uncomment the snippet above -->
{#snippet bar(props: Record<string, unknown>)}{/snippet}

<!-- but not when it's at the bottom -->
<script lang="ts"></script>
