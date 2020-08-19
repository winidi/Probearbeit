<template>
    <footer>
         <div class="footercont">
        <nuxt-link class="footerlinks" to="/admin">
        Admin
        </nuxt-link> 
        <nuxt-link class="footerlinks" id="impressum" to="/kontakt">
        Impressum
        </nuxt-link> 
         </div>
    </footer>
</template>

<style>

#impressum {
 float: left;  
}

.footercont {
  background-color: black;
  
}

.footerlinks {
  float: right;
  color: white;
}

footer {
  text-align: center;
  padding: 1px;
  background-color:brown;
color: #000000;
  float: right;
  width: 100%;
}
</style>