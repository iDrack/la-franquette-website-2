<template>
    <Disclosure as="nav">
      <div class="mx-auto px-2 sm:px-6 lg:px-8">
        <div class="relative flex h-16 items-center justify-between">
          <div class="absolute inset-y-0 left-0 flex items-center">
            <DisclosureButton class="relative inline-flex items-center size-16 justify-center rounded-md p-2 text-gray-900 hover:bg-gray-900 hover:text-white focus:bg-gray-800">
              <span class="absolute -inset-0.5" />
              <span class="sr-only">Ouvrir le menu de navigation</span>
              <Bars3Icon class="block h-6 w-6" aria-hidden="true" />
            </DisclosureButton>
          </div>
        </div>
      </div>
  
      <DisclosurePanel>
        <div class="space-y-1 px-2 pb-3 pt-2">
          <DisclosureButton v-for="item in navigation" :key="item.name" as="a" :href="item.href" :class="[item.current ? 'text-bold' : 'text-gray-300  hover:text-gray-700', 'block rounded-md px-3 py-2']" :aria-current="item.current ? 'page' : undefined">{{ item.name }}</DisclosureButton>
        </div>
      </DisclosurePanel>
    </Disclosure>
  </template>
  
  <script setup>
  import { Disclosure, DisclosureButton, DisclosurePanel} from '@headlessui/vue'
  import { Bars3Icon  } from '@heroicons/vue/24/outline'
  
  const navigation = [
    { name: 'Home', href: '#', current: true },
    { name: 'F.A.Q', href: '/faq', current: false },
    { name: 'Mentions legales', href: '/mentions-legales', current: false },
  ]
  </script>
