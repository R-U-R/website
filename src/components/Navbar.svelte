<script lang="ts">
    import { Icon, ArrowUp, Bars3 } from "svelte-hero-icons";
	import Items from "./Navbar/Items.svelte";
	import Logo from "$components/Logo.svelte";

</script>

<nav class="w-screen fixed top-0 z-40 bg-base-300">
    <!-- TODO: h-16 is a workaround, different sizes on mobile and desktop for some reason -->
    <div class="navbar container mx-auto h-16">
            <div class="navbar-start">
                    <Logo />
            </div>

            <!-- Desktop -->
            <div class="navbar-end menu menu-horizontal hidden lg:flex text-lg">
                    <Items />
            </div>

            <!-- Mobile -->
            <div class="navbar-end lg:hidden">
                    <label for="drawer-checkbox" class="btn btn-square btn-ghost">
                            <!-- <BxMenu class="text-base-100 w-8 h-8" /> -->
                            <Icon src="{Bars3}" class="w-8 h-8" />
                    </label>
            </div>
    </div>
</nav>