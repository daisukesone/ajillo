
<template>
  <el-menu mode="horizontal" :router="true">
    <el-menu-item index="1" style="pointer-events:none;">
      Logo
    </el-menu-item>
    <el-menu-item  index="2" :route="{ hash: '#about' }">
    about us
    </el-menu-item>
    <el-menu-item  index="3" :route="{ hash: '#about' }">
     information
    </el-menu-item>
    <el-menu-item  index="4" :route="{ hash: '#about' }">
    contact
    </el-menu-item>
    <el-menu-item  index="4" :route="{ hash: '#about' }">
    
    </el-menu-item>
  </el-menu>
</template>
