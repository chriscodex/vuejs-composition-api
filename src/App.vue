<script setup lang="ts">
import DinamicComponent from './components/dinamicComponent/DinamicComponent-1.vue';
import Hooks from './components/hooks/Hooks.vue';
import ReactiveExample from './components/reactivity/ReactiveExample.vue';
import ReactiveWatch from './components/reactivity/ReactiveWatch.vue';
import ComputedExample from './components/computed/ComputedExample.vue';
import PropExample from './components/props/PropExample.vue';
import ProvideInjectExample from './components/provideInject/ProvideInjectExample.vue';
import ParentComp from './components/templateRefs/ParentComp.vue';
import ScriptSetup from './components/scripSetup/ScriptSetupExample.vue';
</script>

<template>
  <h3>Dinamic Component</h3>
  <DinamicComponent />
  <h3>Hooks</h3>
  <Hooks />
  <h3>Reactive</h3>
  <ReactiveExample />
  <h3>Reactive Watch</h3>
  <ReactiveWatch />
  <ComputedExample />
  <PropExample first-name="Christian" last-name="Espinoza" />
  <ProvideInjectExample />
  <ParentComp />
  <ScriptSetup first-name="Christian"/>
</template>
