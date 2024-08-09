<!-- This example requires Tailwind CSS v2.0+ -->
<template>
  <Disclosure as="nav" class="my-1" v-slot="{ open }">
    <div class="max-w-7xl mx-auto justify-evenly px-2 sm:px-6 lg:px-8">
      <div class="relative flex items-center justify-between h-16">
        <div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
          <!-- Mobile menu button-->
          <DisclosureButton
              class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-white hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white">
            <span class="sr-only">Open main menu</span>
            <MenuIcon v-if="!open" class="block h-6 w-6" aria-hidden="true"/>
            <XIcon v-else class="block h-6 w-6" aria-hidden="true"/>
          </DisclosureButton>
        </div>
        <div class="flex columns-4 space-x-5 justify-evenly mx-auto sm:items-stretch sm:justify-start">
          <div class="flex-shrink-0 flex items-center">
            <img class="block lg:hidden h-10 w-auto" src="/assets/images/logo.png" alt="Workflow"/>
            <img class="hidden lg:block h-12 mr-6 w-auto" src="/assets/images/logo.png" alt="Workflow"/>
          </div>
          <div class="flex-shrink-0 flex items-center">

            <div class="border-8 p-1.5 rounded-full border-Primary bg-Primary mr-4">
              <i>
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="size-6 fill-white">
                  <path fill-rule="evenodd"
                        d="M1.5 4.5a3 3 0 0 1 3-3h1.372c.86 0 1.61.586 1.819 1.42l1.105 4.423a1.875 1.875 0 0 1-.694 1.955l-1.293.97c-.135.101-.164.249-.126.352a11.285 11.285 0 0 0 6.697 6.697c.103.038.25.009.352-.126l.97-1.293a1.875 1.875 0 0 1 1.955-.694l4.423 1.105c.834.209 1.42.959 1.42 1.82V19.5a3 3 0 0 1-3 3h-2.25C8.552 22.5 1.5 15.448 1.5 6.75V4.5Z"
                        clip-rule="evenodd"/>
                </svg>
              </i></div>
            <div>
              <ul class="text-Accent tracking-wide">Call us on</ul>
              <ul class="text-black font-bold font-mono tracking-tight">+256 753 000 100</ul>
            </div>
          </div>
          <div class="flex-shrink-0 flex items-center">

            <div class="border-8 p-1.5 rounded-full border-Primary bg-Primary mr-4">
              <i>
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="size-6 fill-white">
                  <path fill-rule="evenodd"
                        d="M1.5 4.5a3 3 0 0 1 3-3h1.372c.86 0 1.61.586 1.819 1.42l1.105 4.423a1.875 1.875 0 0 1-.694 1.955l-1.293.97c-.135.101-.164.249-.126.352a11.285 11.285 0 0 0 6.697 6.697c.103.038.25.009.352-.126l.97-1.293a1.875 1.875 0 0 1 1.955-.694l4.423 1.105c.834.209 1.42.959 1.42 1.82V19.5a3 3 0 0 1-3 3h-2.25C8.552 22.5 1.5 15.448 1.5 6.75V4.5Z"
                        clip-rule="evenodd"/>
                </svg>
              </i></div>
            <div>
              <ul class="text-Accent tracking-wide">move@nellions.co.ug</ul>
              <ul class="text-black font-bold font-mono tracking-tight">Mon - Sun, 7AM to 7.30PM</ul>
            </div>
          </div>
          <div class="flex-shrink-0 flex items-center">

            <div class="border-8 p-1.5 rounded-full border-Primary bg-Primary mr-4">
              <i>
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="size-6 fill-white">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" />
                  <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1 1 15 0Z" />
                </svg>
              </i></div>
            <div>
              <ul class="text-Accent tracking-wide">Ntinda Complex, Opp St. Lukes Church</ul>
              <ul class="text-black font-bold font-mono tracking-tight"> Ntinda, Kampala</ul>
            </div>
          </div>
        </div>

      </div>
    </div>


  </Disclosure>
</template>

<script>
import {Disclosure, DisclosureButton, DisclosurePanel, Menu, MenuButton, MenuItem, MenuItems} from '@headlessui/vue'
import {BellIcon, MenuIcon, XIcon} from '@heroicons/vue/outline'

const navigation = [
  {name: 'Dashboard', href: '#', current: true},
  {name: 'Team', href: '#', current: false},
  {name: 'Projects', href: '#', current: false},
  {name: 'Calendar', href: '#', current: false},
]

export default {
  components: {
    Disclosure,
    DisclosureButton,
    DisclosurePanel,
    Menu,
    MenuButton,
    MenuItem,
    MenuItems,
    BellIcon,
    MenuIcon,
    XIcon,
  },
  setup() {
    return {
      navigation,
    }
  },
}
</script>