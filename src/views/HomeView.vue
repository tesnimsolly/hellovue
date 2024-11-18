<template>
  <div class="events">
  <h1> liste des evenements </h1>
       <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src


import EventCard from "@/components/EventCard.vue";

export default {
  components: {
    EventCard,
  },
  data() {
    return {
      events: [
        {
          id: 5928101,
          category: "bien-être animal",
          title: "Journée d'adoption des chats",
          description: "Trouvez votre nouvel ami félin lors de cet événement",
          location: "Meow Town",
          date: "28 January 2022",
          time: "12:00",
          petsAllowed: true,
          organizer: "Foulen Ben Foulen",
        },
         {
          id: 5928101,
          category: "bien-être animal",
          title: "Jardinage",
          description: "Trouvez votre nouvel ami félin lors de cet événement",
          location: "Meow Town",
          date: "28 January 2022",
          time: "12:00",
          petsAllowed: true,
          organizer: "Foulen Ben Foulen",
        },
         {
          id: 5928101,
          category: "bien-être animal",
          title: "nettoyage de plage ",
          description: "Trouvez votre nouvel ami félin lors de cet événement",
          location: "Meow Town",
          date: "28 January 2022",
          time: "12:00",
          petsAllowed: true,
          organizer: "Foulen Ben Foulen",
        },

      ],
    };
  },
};

</script>
<style scoped>
.events{
  display: flex;
 flex-direction: column;
 align-items:center;
}
</style>