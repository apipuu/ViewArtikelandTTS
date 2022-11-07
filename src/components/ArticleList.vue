<template>
  <div
    class="container article-list justify-content-start"
    style="width: fit-content"
  >
    <div class="flex-item">
      <div class="card-title d-flex justify-content-between align-items-center">
        <div>
          <div class="d-flex align-items-center">
            <div class="image-title">
              <img src="../assets/empty pic.png" alt="" />
            </div>
            <div class="px-3">
              <h5 class="mb-0">{{ form.id_user }}</h5>
              <p class="mb-0">Oct 4</p>
            </div>
          </div>
        </div>
        <div>
          <span style="float: right">
            <img src="../assets/save.svg" alt="" />
            <img src="../assets/report.svg" alt="" />
          </span>
        </div>
      </div>
      <h1 class="card-subtitle mt-5">{{ form.judul_artikel }}</h1>
      <p class="card-text w-100 mt-3 text-secondary col-md-6">
        {{ form.deskripsi_artikel }}
      </p>
      <div>
        <img
          src="../assets/poto-artikel.jpg"
          class="img-fluid mt-2"
          alt="..."
        />
      </div>
      <p class="mt-4 description">
        {{ form.isi_artikel }}
      </p>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  name: "App",
  components: {},
  data() {
    return {
      form: {
        id_artikel: "",
        id_user: "",
        cover_artikel: "",
        judul_artikel: "",
        deskripsi_artikel: "",
        isi_artikel: "",
      },
    };
  },
  methods: {
    getItem() {
      axios
        .get("http://localhost:3000/artikel/publish/ART0000000004")
        .then((response) => {
          this.form = response.data;
          console.log(this.form);
        })
        .catch((error) => {
          console.log("Error Get Data ", error);
        });
    },
  },
  mounted() {
    this.getItem();
  },
};
</script>

<style>
.description {
  text-align: justify;
}

.image-title {
  width: 50px;
  height: 50px;
  background-color: #ced4da;
  border-radius: 50%;
}

.image-title img {
  line-height: 50px;
  position: relative;
  margin-left: 4px;
  margin-top: 14px;
}
.article-list {
  display: flex;
  margin-right: 30px;
}

ul {
  list-style: none;
  margin: 0;
  padding: 0;
}
</style>