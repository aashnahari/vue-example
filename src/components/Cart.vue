<script>
import NavBar from './NavBar.vue'
import CartItem from './CartItem.vue'

// Should inherit from app. 
export default {
    data() {
        return {
            hotdog: this.hotdog,
        }
        quantity:0
    },
    props: {
        hotdog: String
    },
    components: {NavBar},

}
</script>

<template>
  <header>
    <NavBar></NavBar>

  </header>
  This is the cart page.
  <main>
    <CartItem>
    <img src="https://images.squarespace-cdn.com/content/v1/5dd8630d09ab5908e35b35a0/1574462664001-48S1VO61L9LNWNJ910CV/img-HotDogStock-1080x675.png?format=1000w" width="200" height="200" />
    <p>Product: Basic Hotdog</p>
    <p> The basic hotdog has no toppings, just the sausage and a bun!</p>
    <p> Price: $2.50</p>
    </CartItem>
    <br>
    <br>
    <CartItem>
    <img src= "https://images.squarespace-cdn.com/content/v1/5dd8630d09ab5908e35b35a0/1575408711651-9RQZJE8ZI0BV3Y1CV0LN/hot+dog+wiht+must.jpg?format=1000w" width="200" height="200" />
    <p>Product: Mustard Hotdog</p>
    <p> The basic hotdog with a topping of mustard!</p>
    <p> Price: $3.50</p>
    </CartItem>
    <br>
    <br>
    <CartItem>
        <img src="https://images.squarespace-cdn.com/content/v1/5dd8630d09ab5908e35b35a0/1582497960940-IAE86F3OGQKE0D19GGYA/ketchup+dog.jpg?format=1000w" width="200" height="200" />
        <p>Product: Ketchup Hotdog</p>
        <p> The basic hotdog with a topping of ketchup!</p>
        <p> Price: $3.50</p>
    </CartItem>
    <br>
    <br>
    <CartItem>
        <img src="https://images.squarespace-cdn.com/content/v1/5dd8630d09ab5908e35b35a0/1586969319681-4OLWCUAYUSSWHGES6IOY/sprinkle+dog.jpg?format=1000w" width = "200" height = "200" />
        <p>Product: Sprinkles Hotdog</p>
        <p> The basic hotdog with a topping of sprinkles!</p>
        <p> Price: $4.00</p>
    </CartItem>
  </main>
</template>

<style scoped>
</style>
