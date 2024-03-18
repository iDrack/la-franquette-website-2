<script>
import emailjs from '@emailjs/browser';

export default {
  methods: {
    sendEmail() {
      emailjs
          .sendForm('service_3dqebpi', 'template_9s00zya', this.$refs.form, {
            publicKey: 's-FO2wleTE-ufyK9b',
          })
          .then(
              () => {
                console.log('SUCCESS!');
              },
              (error) => {
                console.log('FAILED...', error.text);
              },
          );
    },
  },
};
</script>
<template>
    <form ref="form" @submit.prevent="sendEmail" class="ml-auto space-y-4">
        <input type='text' name="user_name" placeholder='Votre nom'
            class="w-full rounded-md py-3 px-2 bg-gray-100 text-sm outline-primary" />
        <input type='email' name="user_email" placeholder='Votre adresse email'
            class="w-full rounded-md py-3 px-2 bg-gray-100 text-sm outline-primary" />
      <input type='tel' name="user_phone" placeholder='Votre numéro de téléphone'
             class="w-full rounded-md py-3 px-2 bg-gray-100 text-sm outline-primary" />
        <textarea name="message" placeholder='Votre message' rows="6"
            class="w-full rounded-md px-4 bg-gray-100 text-sm pt-3 outline-primary"></textarea>
        <div class="flex justify-center">
            <input type='submit'
            class="bg-secondary text-white font-bold rounded-md text-sm px-4 py-3" value="Prendre contact"/>
        </div>
    </form>


</template>

<style scoped>
</style>