<script lang="ts">
	import { Section, ForgotPassword, ForgotPasswordHeader } from 'flowbite-svelte-blocks';
	import { Label, Input, Button, Checkbox } from 'flowbite-svelte';
</script>

<Section name="forgotpassword">
	<ForgotPasswordHeader src="/images/logo/pelni-logo-gram.png" alt="logo" href="/"
		>{null}</ForgotPasswordHeader
	>
	<ForgotPassword>
		<h1
			class="mb-1 text-xl leading-tight font-bold tracking-tight text-gray-900 md:text-2xl dark:text-white"
		>
			Forgot your password?
		</h1>
		<p class="font-light text-gray-500 dark:text-gray-400">
			Don't fret! Just type in your email and we will send you a code to reset your password!
		</p>
		<form class="mt-4 space-y-4 md:space-y-5 lg:mt-5">
			<div>
				<Label for="email" class="mb-2 block text-sm font-medium text-gray-900 dark:text-white"
					>Your email</Label
				>
				<Input type="email" name="email" id="email" placeholder="name@company.com" required />
			</div>
			<div class="flex items-start">
				<div class="flex h-5 items-center">
					<Checkbox id="terms" aria-describedby="terms" required>
						I accept the <a
							class="text-primary-600 dark:text-primary-500 font-medium hover:underline"
							href="/">Terms and Conditions</a
						>
					</Checkbox>
				</div>
			</div>
			<Button type="submit" color="red">Reset password</Button>
		</form>
	</ForgotPassword>
</Section>
