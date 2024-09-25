<script setup lang="ts">
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { Head } from '@inertiajs/vue3';
import Tunnel from "@/Symbols/Tunnel.vue";
import Factory from "@/Symbols/Factory.vue";
</script>

<template>
	<Head title="Board" />
	<AuthenticatedLayout>
		<template #header>
			<h2 class="font-semibold text-xl text-gray-800 dark:text-gray-200 leading-tight">Sense Board</h2>
		</template>
		<div class="board text-center ">
			<div class="sensemap">
				<div class="rows shift">
					<div class="tile invisible"></div>
					<div class="tile">A0</div>
					<div class="tile invisible"></div>
					<div class="tile invisible"></div>
					<div class="tile">D0</div>
					<div class="tile invisible"></div>
					<div class="tile invisible"></div>
					<div class="tile invisible"></div>
				</div>
				<div class="rows">
					<div class="tile invisible"></div>
					<div class="tile">A1</div>
					<div class="tile">B1</div>
					<div class="tile">C1</div>
					<div class="tile">D1</div>
					<div class="tile">E1</div>
					<div class="tile">F1</div>
					<div class="tile invisible"></div>
				</div>

				<div class="rows shift">
					<div class="tile">A2</div>
					<div class="tile">B2</div>
					<div class="tile">C2</div>
					<div class="tile">D2
						<Tunnel/>
					</div>
					<div class="tile">E2</div>
					<div class="tile">F2</div>
					<div class="tile">G2</div>
				</div>
				<div class="rows">
					<div class="tile">A3</div>
					<div class="tile">B3</div>
					<div class="tile">C3
						<Tunnel/>
					</div>
					<div class="tile">D3</div>
					<div class="tile">E3</div>
					<div class="tile">F3
						<Tunnel/>
					</div>
					<div class="tile">G3</div>
					<div class="tile">H3</div>
				</div>
				<div class="rows shift">
					<div class="tile">B4</div>
					<div class="tile">C4</div>
					<div class="tile">D4</div>
					<div class="tile">E4
						<Factory />
					</div>
					<div class="tile">F4</div>
					<div class="tile">G4</div>
					<div class="tile">H4</div>
				</div>
				<div class="rows">
					<div class="tile">B5</div>
					<div class="tile">C5</div>
					<div class="tile">D5
						<Tunnel/>
					</div>
					<div class="tile">E5</div>
					<div class="tile">F5</div>
					<div class="tile">G5
						<Tunnel/>
					</div>
					<div class="tile">H5</div>
				</div>
				<div class="rows shift">
					<div class="tile">C6</div>
					<div class="tile">D6</div>
					<div class="tile">E6</div>
					<div class="tile">F6
						<Tunnel/>
					</div>
					<div class="tile">G6</div>
					<div class="tile">H6</div>
					<div class="tile">I6</div>
				</div>
				<div class="rows">
					<div class="tile">C7</div>
					<div class="tile">D7</div>
					<div class="tile">E7</div>
					<div class="tile">F7</div>
					<div class="tile">G7</div>
					<div class="tile">H7</div>
					<div class="tile">I7</div>
					<div class="tile">J7</div>
				</div>
				<div class="rows shift">
					<div class="tile invisible"></div>
					<div class="tile invisible"></div>
					<div class="tile">F8</div>
					<div class="tile">G8</div>
				</div>
			</div>
		</div>
	</AuthenticatedLayout>
</template>
