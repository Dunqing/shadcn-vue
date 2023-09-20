---
title: Command
description: Fast, composable, unstyled command menu.
source: apps/www/src/lib/registry/default/ui/command 
primitive: https://www.radix-vue.com/components/combobox.html
---


<ComponentPreview name="CommandDemo" /> 



## Installation

 
```bash
npx shadcn-vue@latest add command
``` 
## Usage

```vue
<script setup lang="ts">
import {
  Command,
  CommandDialog,
  CommandEmpty,
  CommandGroup,
  CommandInput,
  CommandItem,
  CommandList,
  CommandSeparator,
  CommandShortcut,
} from '@/components/ui/command'
</script>

<template>
  <Command>
    <CommandInput placeholder="Type a command or search..." />
    <CommandList>
      <CommandEmpty>No results found.</CommandEmpty>
      <CommandGroup heading="Suggestions">
        <CommandItem>Calendar</CommandItem>
        <CommandItem>Search Emoji</CommandItem>
        <CommandItem>Calculator</CommandItem>
      </CommandGroup>
      <CommandSeparator />
      <CommandGroup heading="Settings">
        <CommandItem>Profile</CommandItem>
        <CommandItem>Billing</CommandItem>
        <CommandItem>Settings</CommandItem>
      </CommandGroup>
    </CommandList>
  </Command>
</template>```