<template>
  <div class="article">
     <div>
         <h4>{{ productName }}</h4>
         <p>Quantité: {{ productQuantity }}</p>
     </div>
     <div>
        <img class="images" :src="img" alt="image produit">
     </div>
   </div>
</template>

<script>
export default {
   name: 'Shopping',
   props: {
      productName: String,
      productQuantity: Number,
      img: String
   }
}
</script>

<style scoped>
   .article {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 0;
      border-bottom: 1px solid orange;
      text-align: left;
      line-height: 0.5rem;
      color: rgb(161, 161, 161);
   }

   .images {
      width: 70px;
      height: auto;
      margin-right: 1rem;
   }
</style>