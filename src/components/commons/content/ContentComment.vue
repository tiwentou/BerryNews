<template>
  <div class="content-comment">
    <div class="content-comment-header">{{ count() }} Commentaires</div>
    <div class="content-comment-container">
      <div class="content-comment-item" v-for="(item, index) in comments" v-bind:key="index">
        <Comment :index="item.index" :username="item.username" :text="item.text" />
      </div>
      <div class="comment-content-form-add">
        <input type="text" placeholder="Ton username..." v-model="formCommentUsername" />
        <textarea
          name="comment"
          id="add-comment-text"
          cols="30"
          rows="3"
          placeholder="Commente par ici ..."
          v-model="formCommentText"
        ></textarea>
        <a href="#" @click="send">Envoyer</a>
      </div>
    </div>
  </div>
</template>

<script>
import Comment from "@/components/commons/comment/Comment.vue";

export default {
  name: "ContentComment",
  components: {
    Comment
  },
  data() {
    return {
      comments: [],
      formCommentUsername: "",
      formCommentText: ""
    };
  },
  methods: {
    count() {
      return this.comments.length;
    },
    send(e) {
      let comment = {
        index: this.count() + 1,
        username: this.formCommentUsername,
        text: this.formCommentText
      };
      this.comments.push(comment);
      this.resetField();
      e.preventDefault();
    },
    resetField() {
      this.formCommentUsername = "";
      this.formCommentText = "";
    }
  }
};
</script>

<style scoped>
.content-comment .content-comment-header {
  background-color: #40565e;
  color: white;

  padding: 10px;
  padding-left: 20px;

  font-size: 1.5em;
}

.content-comment .content-comment-container {
  padding: 40px;
}

.content-comment .content-comment-item {
  margin-top: 10px;
}

.content-comment .comment-content-form-add {
  margin-top: 40px;
  margin-bottom: 40px;
}

.content-comment .comment-content-form-add input {
  width: 20%;
  padding: 10px;
  padding-left: 20px;
  background-color: #cdd8dc;
  border-style: none;
  border: #9b9b9b solid 1px;
}

.content-comment .comment-content-form-add textarea {
  resize: none;
  width: 100%;

  margin-top: 10px;
  padding: 20px;

  box-sizing: border-box;

  background-color: #cdd8dc;
}

.content-comment .comment-content-form-add a{ 
    float: right;
    background-color: #167DAC;
    padding: 8px;
    margin-top: 10px;
}
</style>
