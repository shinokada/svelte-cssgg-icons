<script>
  import '../app.postcss';
  import { page } from '$app/stores';
  import DarkMode from 'flowbite-svelte/DarkMode.svelte';
  import Navbar from 'flowbite-svelte/Navbar.svelte';
  import NavBrand from 'flowbite-svelte/NavBrand.svelte';
  import NavLi from 'flowbite-svelte/NavLi.svelte';
  import NavUl from 'flowbite-svelte/NavUl.svelte';
  import NavHamburger from 'flowbite-svelte/NavHamburger.svelte';
  import Footer from 'flowbite-svelte/Footer.svelte'
  import FooterBrand from 'flowbite-svelte/FooterBrand.svelte'
  import FooterLinkGroup from 'flowbite-svelte/FooterLinkGroup.svelte'
  import FooterLink from 'flowbite-svelte/FooterLink.svelte'
  import { MetaTags } from 'svelte-meta-tags';

  $: activeUrl = $page.url.pathname;
</script>

<MetaTags
  title="Svelte Cssgg Icons"
  description="svelte-cssgg-icons icon set for Svelte"
  openGraph={{
    type: 'website',
    url: 'https://svelte-cssgg-icons.vercel.app/',
    title: "Svelte Cssgg Icons",
    description: "Cssgg icon set for Svelte",
    images: [{ url: 'https://open-graph-vercel.vercel.app/api/svelte-cssgg-icons', width: 1200, height: 630, alt: "Svelte Cssgg Icons" }],
    site_name: 'Svelte Cssgg Icons'
  }}
  twitter={{
    handle: '@shinokada',
    cardType: 'summary_large_image',
    title: "Svelte Cssgg Icons",
    description: "Cssgg icon set for Svelte",
    image:'https://open-graph-vercel.vercel.app/api/svelte-cssgg-icons',
    imageAlt: "Svelte Cssgg Icons"
  }} />
  
<Navbar let:hidden let:toggle class="dark:bg-zinc-900">
  <NavBrand href="/">
    <span class="self-center whitespace-nowrap text-2xl font-semibold text-primary-700 dark:text-primary-500">
      Svelte Cssgg Icons
    </span>
  </NavBrand>
  <NavHamburger on:click={toggle} />
  <NavUl {hidden}>
    <NavLi href="/" active={activeUrl === '/'}>Home</NavLi>
    <NavLi href="/icons" active={activeUrl === '/icons'}>Icons</NavLi>
    <NavLi href="https://github.com/shinokada/svelte-cssgg-icons">GitHub</NavLi>
    <NavLi href="https://svelte-svg-icons.vercel.app/">Icon sets</NavLi>
  </NavUl>
  <DarkMode />
</Navbar>
<div class="mx-16 mb-16">
  <slot />
</div>

<Footer footerType="logo" class="dark:bg-zinc-900 mx-8">
  <div class="sm:flex sm:items-center sm:justify-between">
  <FooterBrand
  href="https://svelte-cssgg-icons.vercel.app/"
  name="Svelte Cssgg Icons"
/>
  <FooterLinkGroup ulClass="flex flex-wrap items-center mt-3 text-sm text-gray-500 dark:text-gray-400 sm:mt-0">
    <FooterLink href="/docs">Docs</FooterLink>
    <FooterLink href="https://github.com/shinokada/svelte-cssgg-icons/blob/main/LICENSE">Licensing</FooterLink>
    <FooterLink href="https://github.com/shinokada/svelte-cssgg-icons/">GitHub</FooterLink>
  </FooterLinkGroup>
  </div>
</Footer>

