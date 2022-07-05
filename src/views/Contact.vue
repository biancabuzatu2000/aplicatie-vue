<template>
    <main class="contact-page">
        <h1>Contactează-ne: </h1>
        <form @submit.prevent="handleSubmit">
            <label for="name">
                name:
                <input id="name" text="text" >
            </label>
            <label for="msg">
            message:
            <textarea id="msg" />
            </label>
            <button>
                Trimite mesajul
            </button>
        </form>
    </main>
</template>

<script>
    export default {
        name: 'Contact',
        methods: {
            handleSubmit () {
                console.log('send detail to server')
            }
        }
    }
</script>

<style lang="scss">
    .contact-page {
        form {
            
            margin: 0 auto;
            text-align: left;
            width: 300px;
            border-radius: 17px;

        label {
            display: block;
            }
        input, textarea {
            display: block;
            width: 100%;
            resize: none;
            }
        button {
            padding: 11px 20px;
            border-radius: 7px;
            display: block;
            margin-left: auto;
            color: white;
            margin-top: 20px;
            background-color: #ffb3b3;
            border: none;
            }
        }
    }
</style>
