<script lang="ts">
	import { counter } from '../spa.svelte';
	import { base } from '$app/paths';
</script>

<h1>WOW</h1>
<p>
	Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi imperdiet velit elit, sit amet
	pellentesque sem tempor quis. Maecenas consequat lorem lectus, eget pharetra urna pretium vel.
	Vivamus vel fermentum risus, a laoreet lectus. Morbi eu lobortis est, nec porttitor est. Aliquam
	vel feugiat nisl. In rutrum diam id rhoncus accumsan. Cras dignissim facilisis turpis non auctor.
	Mauris cursus, eros in vestibulum viverra, mi tortor lacinia enim, nec mollis metus elit eget mi.
	Vestibulum justo nisi, imperdiet in sagittis sit amet, interdum nec massa.
</p>
<p><a href="{base}/spa/yay">yay page</a>yay</p>

<div class="counter">counter: {counter.num}</div>

<button
	onclick={() => {
		counter.num += 1;
	}}>+</button
>

<button
	onclick={() => {
		counter.num -= 1;
	}}>-</button
>

<style>
	button {
		/*폰트의 크기를 수정하냐 안하냐에 따라서 단위를 rem을 쓸지 px를 쓸지 달라진다*/
		/*폰트 크기 조정시 px 아니면 rem*/
		/*font-size: 20px;*/
		width: 4rem;
		height: 1.5rem;
	}
</style>
