<template>
  <div style="padding-top:150px" class="row flex justify-around">
    <q-card class="my-card col-3">
      <q-card-section class="bg-light-blue-8 text-white">
        <div class="text-h6">Donors</div>
        <div class="text-subtitle2">Number of Donors</div>
      </q-card-section>

      <q-separator />

      <q-card-section
        class="flex flex-center"
        style="font-size:36px"
      >
        <div> {{numberOfDonors}} </div>
      </q-card-section>
    </q-card>
    <q-card class="my-card col-3">
      <q-card-section class="bg-deep-purple-8 text-white">
        <div class="text-h6">Our Changing Planet</div>
        <div class="text-subtitle2">by John Doe</div>
      </q-card-section>

      <q-separator />

      <q-card-actions align="right">
        <q-btn flat>Action 1</q-btn>
        <q-btn flat>Action 2</q-btn>
      </q-card-actions>
    </q-card>
    <q-card class="my-card col-3">
      <q-card-section class="bg-deep-orange-8 text-white">
        <div class="text-h6">Our Changing Planet</div>
        <div class="text-subtitle2">by John Doe</div>
      </q-card-section>

      <q-separator />

      <q-card-actions align="right">
        <q-btn flat>Action 1</q-btn>
        <q-btn flat>Action 2</q-btn>
      </q-card-actions>
    </q-card>
  </div>
</template>

<script>
export default {
  data() {
    return {
      numberOfDonors: '500 Donors'
    };
  }
};
</script>

<style scoped></style>
