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
              <h5 class="mb-0">Contributor Name</h5>
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
      <h1 class="card-subtitle mt-5">Article Title</h1>
      <p class="card-text w-100 mt-3 text-secondary col-md-6">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam veroquos,
        saepe atque quae nostrum numquam sequi quis minus laboriosam, repellat,
        ipsum voluptatem laudantium perspiciatis facilis.
      </p>
      <div>
        <img
          src="../assets/poto-artikel.jpg"
          class="img-fluid mt-2"
          alt="..."
        />
      </div>
      <p class="mt-4 description">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Amet, viverra
        mauris sociis velit eget non. Consectetur volutpat adipiscing quam amet
        tellus gravida habitant sit. Sed nunc aliquam sagittis ultricies vel
        quam ut diam sit. Tristique enim netus sed cursus in quis. Montes, fames
        a mauris tristique viverra risus. Purus eget pretium pellentesque a,
        turpis. Mi enim, morbi egestas sed. Morbi ac eleifend vulputate massa
        maecenas adipiscing vestibulum elementum. In id quis in ut et. Egestas
        justo sit eu enim proin ut massa. Tincidunt donec pharetra amet sed.
        Scelerisque et non euismod consequat. Lacus, ultrices tristique amet
        adipiscing commodo ut. Est dignissim mi odio sit. Enim potenti varius
        lobortis blandit velit ut aliquet. Iaculis donec cursus nam aenean nulla
        semper. Arcu sapien sed dictum magna ultrices eget morbi risus in. Est
        in orci eu faucibus malesuada euismod. Blandit eget mauris, integer
        viverra consequat. Imperdiet tincidunt venenatis interdum ac, imperdiet
        euismod nibh aliquam semper. Maecenas lobortis molestie et netus. In et
        libero eget aliquet sagittis venenatis ut. Dolor vivamus magna arcu quam
        elementum arcu risus, turpis. Quam in ac vitae proin ornare scelerisque
        a vel. Mattis enim sagittis, netus sit. Et nibh molestie pretium nulla
        vitae malesuada ornare hendrerit.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
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