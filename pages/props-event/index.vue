<template>
    <div>
        <top-component/>
        <main-component/>
        <bottom-component/>
    </div>
</template>
<script>
import TopComponent from '../../components/ChildComponent/TopComponent.vue';
import BottomComponent from '../../components/ChildComponent/BottomComponent.vue';
import MainComponent from '../../components/ChildComponent/MainComponent.vue';

export default {
    components: {TopComponent,BottomComponent,MainComponent}
}

</script>