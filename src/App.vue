<<template>
  <div>
    <div>
      <h1>Participants list</h1>
      <ol v-if="participants.length() > 0 ">
        <li :key="number" v-for="number in participants">{{}}</li>
      </ol>
    </div>

    <h3>New participant</h3>
    <form @submit.prevent="addNewParticipant()">
      <label>Firstname</label>
      <input type="text">
      <label>Lastname</label>
      <input type="text">
      <button>Add new participant</button>
    </form>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        participants:[]
      };
    },
    methods: {
      addNewParticipant() {
        this.participant.push();
      }
    }
  };
</script>


