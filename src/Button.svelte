<script></script>

<button class="btn-fill btn-primary-2">
	<slot></slot>
</button>

<style>
	.btn-fill {
		width: 100%;
	}

	.btn-primary-2 {
		border: none;
		border-radius: 6px;

		color: var(--neutral-1);
		background-color: var(--primary-2);
		padding: 14px 0;

		box-shadow: 0 3px 6px rgba(0, 0, 0, 0.16), 0 3px 6px rgba(0, 0, 0, 0.23);
	}
</style>
