<template>
  <ul class="list-group">
    <li class="list-group-item">
      <button
        type="button"
        class="close"
        data-dismiss="modal"
        aria-label="Close"
      >
        <span aria-hidden="true">&times;</span>
      </button>
      <div class="media-body">
        <img
          width="80px"
          src="https://m.media-amazon.com/images/I/719tCHXNiXL._AC_UL320_.jpg"
          class="mr-3"
          alt="..."
        />
        <div class="media-body">
          <p class="mt-0">Judul</p>
          <button class="btn-qty btn btn-sm btn-secondary">-</button>
          dapp
          <button class="btn-qty btn btn-sm btn-secondary">+</button>
        </div>
      </div>
    </li>
  </ul>
</template>

<style scoped>
.btn-qty {
  border-radius: 45%;
  width: 35px;
}

.media{
     width:90%; 
}
.media-body {
  text-align: left;
}
</style>
