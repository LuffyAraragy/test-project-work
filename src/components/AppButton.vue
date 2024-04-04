<template>
    <button 
        class="app-button"
        :class="innerClass"
    >
        <slot class="text-button">
            {{ text }}
        </slot>
    </button>
    </template>
    
    <script>
    export default {
        name: 'AppButton',
        props: {
            disabled: Boolean,
            hasOutline: Boolean,
            hasWhite: Boolean,
            hasBlack: Boolean,
            hasSmall: Boolean,
            hasGreen: Boolean,
            hasAround: Boolean,
            width: {
                type: String,
                default: ''
            },
            text: {
                type: String,
                default: 'Button'
            }
        },
        computed: {
            innerClass() {
                return {
                    '--outline': this.hasOutline,
                    '--white': this.hasWhite,
                    '--black': this.hasBlack,
                    '--custom-width': this.width,
                    '--small': this.hasSmall,
                    '--rounded': this.hasRounded,
                    '--green': this.hasGreen,
                    '--border-around': this.hasAround,
                }
            }
        }
    }
    </script>
    
    <style lang="scss">
    @import '../assets/variables.scss';

    .app-button {
        //Базовое поведение кнопки

        &.--white:hover {
            border: $border-size-4 solid $color-green;
        }

        &.--white:focus {
            color: $color-white;
            background: $color-green-black;
        } 
    }
    </style>