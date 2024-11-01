# Button

<script >

import Btn from '../../../ui/src/components/button/Core.vue'; 
</script>

**Button with Custom Effect**

<div class="border-[1px] border-gray-300 p-6 rounded-lg shadow-inner bg-white flex justify-center items-center ">
    <Btn color="default">Test</Btn>
</div>

**Customize the color as you like or use the default values!**
<Br/>

<div class="grid grid-cols-2 gap-4">
    <div class="border-[1px] border-gray-300 p-4 rounded-lg shadow-inner bg-white flex justify-center items-center">
        <Btn color="default" class="w-[125px]">Default</Btn>
    </div>
    <div class="border-[1px] border-gray-300 p-4 rounded-lg shadow-inner bg-white flex justify-center items-center">
        <Btn color="primary">Primary</Btn>
    </div>
    <div class="border-[1px] border-gray-300 p-4 rounded-lg shadow-inner bg-white flex justify-center items-center">
        <Btn color="error"> Error !!</Btn>
    </div>
    <div class="border-[1px] border-gray-300 p-4 rounded-lg shadow-inner bg-white flex justify-center items-center">
        <Btn color="warning">Warning</Btn>
    </div>
    <div class="border-[1px] border-gray-300 p-4 rounded-lg shadow-inner bg-white flex justify-center items-center">
        <Btn color="secondary">Second</Btn>
    </div>
    <div class="border-[1px] border-gray-300 p-4 rounded-lg shadow-inner bg-white flex justify-center items-center">
        <Btn color="gradient">Gradient</Btn>
    </div>
</div>
<Br/>
<Br/>

#Code 



The main `<Btn>` tag can be call and using button

```md
<template>

<Btn color="warning" @click="handleError">you have notification</Btn>

<script >
const handleError = () => {
    alert("test");
}
</script>
```
Results

<div class='border-[1px] border-gray-300 p-4 rounded-lg shadow-inner bg-white flex justify-center items-center'>
  <Btn color="warning" @click="handleError">You have a notification!</Btn>
</div>

<script setup>
const handleError = () => {
  alert("Test notification triggered!");
}
</script>

-----------------
**Disable**

You Can use   *isDisable*  for disable your button
<div class='border-[1px] border-gray-300 p-4 rounded-lg shadow-inner bg-white flex justify-center items-center'>

<Btn  isDisabled>Disabled </Btn>


</div>

```md
<Btn  isDisabled >Disabled </Btn>
```
---



**Link Button**
<div class='border-[1px] border-gray-300 p-4 rounded-lg shadow-inner bg-white flex justify-center items-center flex flex-row'>
<Btn  color ="link" > link  </Btn>

</div>

```md
<Btn  color ="link" > link  </Btn>


```


**Also You can Use with Icons**
<div class='border-[1px] border-gray-300 p-4 rounded-lg shadow-inner bg-white flex justify-center items-center flex flex-row'>
    <Btn color="secondary"> <!-- Use space-x-2 for spacing -->
        <span>waiting</span>
        <div class="scale-50">
        <svg class="animate-spin" role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
            <path d="M11.71 0C8.24 3.9 6.92 6 6.64 9.14c-.01-.01-.03-.01-.04-.02-1.28-.73-2.3-2.22-2.91-3.73l-2.23.87c1.64 4.95 2.81 7.13 5.39 8.94-.02.01-.03.02-.05.03-1.27.74-3.07.89-4.68.66l-.36 2.37c5.11 1.06 7.59 1.15 10.46-.19v.06c0 1.47-.77 3.09-1.78 4.38L12.3 24c3.46-3.89 4.78-5.99 5.06-9.13.02.01.03.01.05.02 1.27.73 2.29 2.21 2.9 3.73l2.23-.87c-1.64-4.95-2.8-7.14-5.39-8.95.02-.01.03-.02.05-.03 1.27-.74 3.07-.88 4.68-.65l.36-2.38c-5.1-1.06-7.58-1.14-10.44.19v-.06c0-1.47.77-3.09 1.78-4.38L11.71 0zm.19 8.82a3.181 3.181 0 0 1 3.28 3.07 3.181 3.181 0 0 1-3.07 3.28 3.181 3.181 0 0 1-3.28-3.07 3.181 3.181 0 0 1 3.07-3.28z"/>
</svg>
</div>
</Btn>
</div>

<br/>