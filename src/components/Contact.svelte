<script lang="ts">
    import { Icon, Home, Phone, AtSymbol } from "svelte-hero-icons";

    let contacts = [
        [AtSymbol,],
        [Phone,],
        [Home,],
    ];
</script>

<div class="w-full py-8" id="contact">
	<div class="container mx-auto px-2">
		<h3 class="text-4xl font-bold text-center mb-2">Kontakt</h3>
		<div class="flex">
			{#each contacts as contact}
				<div class="w-full">
                    <Icon src="{contact[0]}" class="max-w-32 w-full mx-auto"/>
				</div>
			{/each}
		</div>
	</div>
</div>
