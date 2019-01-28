<template lang="html">
  <transition name="modal">
    <div class="modal-mask">
      <div class="modal-wrapper">
        <div class="modal-container">
          <div class="modal-header">
            <slot name="header">
              {{getPrizeName()}}
            </slot>
          </div>

          <div class="modal-body">
            <slot name="body">
              {{getPrizeDesc()}}
            </slot>
          </div>

          <div class="modal-footer">
            <slot name="footer">
              {{prizeFooter}}
              <button class="modal-default-button" @click="$emit('close')">
                OK
              </button>
            </slot>
          </div>
        </div>
      </div>
    </div>
  </transition>
</template>

<script>
export default {
  props: {
    prizeName:  String,
    prizeDesc:  String,
    prizeFooter: String
  },
  methods: {
    getPrizeName(){
      if (this.prizeName) {
        return this.prizeName
      }
      else {
        return 'CONGRATULATIONS!'
      }
    },
    getPrizeDesc(){
      if (this.prizeDesc) {
        return this.prizeDesc
      }
      else {
        return 'Description...'
      }
    },
  }
}
</script>

<style lang="css">
.modal-mask {
  position: fixed;
  z-index: 9998;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, .5);
  display: table;
  transition: opacity .3s ease;
}

.modal-wrapper {
  display: table-cell;
  vertical-align: middle;
}

.modal-container {
  width: 300px;
  height: 300px;
  scroll: auto;
  margin: 0px auto;
  padding: 20px 30px;
  background-color: #fff;
  border: 4px solid black;
  border-radius: 2px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, .33);
  transition: all .3s ease;
  font-family: Helvetica, Arial, sans-serif;
}

.modal-header {
  margin-top: 0;
  color: #42b983;
}

.modal-body {
  margin: 20px 0;
}

.modal-default-button {
  margin: 200px 0 0 0;
}

/*
 * The following styles are auto-applied to elements with
 * transition="modal" when their visibility is toggled
 * by Vue.js.
 *
 * You can easily play with the modal transition by editing
 * these styles.
 */

.modal-enter {
  opacity: 0;
}

.modal-leave-active {
  opacity: 0;
}

.modal-enter .modal-container,
.modal-leave-active .modal-container {
  -webkit-transform: scale(1.1);
  transform: scale(1.1);
}
</style>
