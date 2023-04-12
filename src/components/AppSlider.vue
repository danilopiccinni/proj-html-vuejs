<script>
export default {
  data() {
    return {
      offset: -1550,
      step: 150 // la larghezza di ogni immagine
    };
  },
  methods: {
    scroll(direction) {
      this.offset += this.step * direction;
    }
  },


};
</script>

<template>
    <div class="slider-laterale">
      <div class="slider-content" :style="{ transform: 'translateX(' + offset + 'px)' }">
        <slot></slot>
      </div>
      <div class="slider-controls">
        <button @click="scroll(3)"><i class="fa-solid fa-circle-chevron-left"></i></button>
        <button @click="scroll(-3)"><i class="fa-solid fa-circle-chevron-right"></i></button>
      </div>
    </div>
  </template>
  
  <style scoped lang="scss">
  .slider-laterale {
    padding-bottom: 50px;
    position: relative;
    overflow: hidden;
    
  }
  .slider-content {
    display: flex;
    justify-content: center;
    gap: 25px;
    transition: transform 0.5s;
  }
  .slider-controls {

    position: absolute;
    bottom: -5px;
    right: 50%;
    transform: translateX(50%);
  
  }
  .slider-controls button {
    background-color: transparent;
    color: #1675bf;
    border: none;

    font-size: 2rem;
    padding: 0 1rem;
    cursor: pointer;

    &:hover {
      color: #2e9cf0;
    }
  }
  </style>