<script setup lang="ts">
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { Head } from '@inertiajs/vue3';
import Tunnel from "@/Symbols/Tunnel.vue";
import Factory from "@/Symbols/Factory.vue";
import Tile from "@/Symbols/Tile.vue";
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
					<Tile id="a0"/>
					<div class="tile invisible"></div>
					<div class="tile invisible"></div>
					<Tile id="d0"/>
					<div class="tile invisible"></div>
					<div class="tile invisible"></div>
					<div class="tile invisible"></div>
				</div>
				<div class="rows">
					<div class="tile invisible"></div>
					<Tile id="a1"/>
					<Tile id="b1"/>
					<Tile id="c1"/>
					<Tile id="d1"/>
					<Tile id="e1"/>
					<Tile id="f1"/>
					<div class="tile invisible"></div>
				</div>

				<div class="rows shift">
					<Tile id="a2"/>
					<Tile id="b2"/>
					<Tile id="c2"/>
					<Tile id="d2">
						<Tunnel/>
					</Tile>
					<Tile id="e2"/>
					<Tile id="f2"/>
					<Tile id="g2"/>
				</div>
				<div class="rows">
					<Tile id="a3"/>
					<Tile id="b4"/>
					<Tile id="c3">
						<Tunnel/>
					</Tile>
					<Tile id="d3"/>
					<Tile id="e3"/>
					<Tile id="f3">
						<Tunnel/>
					</Tile>
					<div id="tile-g3" class="tile">G3</div>
					<div id="tile-h3" class="tile">H3</div>
				</div>
				<div class="rows shift">
					<div id="tile-b4" class="tile">B4</div>
					<div id="tile-c4" class="tile">C4</div>
					<div id="tile-d4" class="tile">D4</div>
					<div id="tile-e4" class="tile">E4
						<Factory />
					</div>
					<div id="tile-f4" class="tile">F4</div>
					<div id="tile-g4" class="tile">G4</div>
					<div id="tile-h4" class="tile">H4</div>
				</div>
				<div class="rows">
					<div id="tile-b5" class="tile">B5</div>
					<div id="tile-c5" class="tile">C5</div>
					<div id="tile-d5" class="tile">D5
						<Tunnel/>
					</div>
					<div id="tile-e5" class="tile">E5</div>
					<div id="tile-f5" class="tile">F5</div>
					<div id="tile-g5" class="tile">G5
						<Tunnel/>
					</div>
					<div id="tile-h5" class="tile">H5</div>
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
