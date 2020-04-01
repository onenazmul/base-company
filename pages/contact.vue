<template>
  <div class="inner-content">
    <b-container>
      <b-row>
        <b-col class="text-center mb-4">
          <h1>Let's get connected</h1>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod
            voluptatem incidunt eos repellat hic quas dolores tenetur expedita
            ratione neque.
          </p>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <b-form v-if="show" netlify @submit="onSubmit">
            <b-form-group
              id="input-group-2"
              label="Your Name:"
              label-for="input-2"
            >
              <b-form-input
                id="input-2"
                v-model="form.name"
                required
                placeholder="Enter name"
              ></b-form-input>
            </b-form-group>
            <b-form-group
              id="input-group-1"
              label="Email address:"
              label-for="input-1"
              description="We'll never share your email with anyone else."
            >
              <b-form-input
                id="input-1"
                v-model="form.email"
                type="email"
                required
                placeholder="Enter email"
              ></b-form-input>
            </b-form-group>
            <b-form-group
              id="input-group-4"
              label="Phone Number:"
              label-for="input-4"
              description="We'll never share your phone number with anyone else."
            >
              <b-form-input
                id="input-4"
                v-model="form.phone"
                type="tel"
                required
                placeholder="Enter phone"
              ></b-form-input>
            </b-form-group>
            <b-form-group
              id="input-group-3"
              label="Interest:"
              label-for="input-3"
            >
              <b-form-select
                id="input-3"
                v-model="form.food"
                :options="foods"
                required
              ></b-form-select>
            </b-form-group>
            <b-button type="submit" variant="primary">Submit</b-button>
          </b-form>
        </b-col>
        <b-col>
          <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3651.854773148267!2d90.37867221486079!3d23.752557684588286!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3755b9f7e9a6c3b3%3A0x61956801bb9b9e4a!2sDynasty%20Wahed%20Tower!5e0!3m2!1sen!2sbd!4v1584902777028!5m2!1sen!2sbd"
            width="100%"
            height="450"
            frameborder="0"
            style="border:0;"
            allowfullscreen
            aria-hidden="false"
            tabindex="0"
          ></iframe>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  /* eslint-disable */
  data() {
    return {
      form: {
        email: '',
        name: '',
        phone: '',
        food: null
      },
      foods: [
        { text: 'Pick a topic', value: null },
        'Courses',
        'Web Services',
        'Other'
      ],
      show: true
    }
  },
  methods: {
    onSubmit(evt) {
      evt.preventDefault()
      alert('Thanks for submitting!')
      this.form.email = ''
      this.form.name = ''
      this.form.food = null
      this.form.phone = ''
    }
  },
  head: {
    title: 'Contact Us'
  }
}
</script>

<style></style>
