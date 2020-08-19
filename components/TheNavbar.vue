<template>
    <div class="thenavbar">
      <ul>
          <li>
        <nuxt-link class="links" to="/">
        LeosRestaurant
        </nuxt-link> 
          </li>
          <li>
        <nuxt-link class="links" to="/historie">
        Historie
        </nuxt-link> 
          </li>
        <nuxt-link class="links" to="/kontakt">
        Kontakt
        </nuxt-link>
        <nuxt-link class="links" to="/speisekarte">
        Speisekarte
        </nuxt-link> 
        <nuxt-link class="links" id="gaestebuchlink" to="/gaestebuch">
        Gästebuch
        </nuxt-link>
      </ul>
    </div>
</template>

<style>

    #gaestebuchlink{
        float: right;
    }

    .links{
  
        float: left;
    
    }

    ul {
        list-style-type: none;
        margin: 0;
        padding: 0;
        overflow: hidden;
    }

    .thenavbar {
      font-family: 'Times New Roman', Times, serif;
      font-weight: 700;
      font-size: 1.5em;
      color: #000000;
      text-decoration: none;
      background-color: brown;
    }
    
    .links{
        display: block;
        color: rgb(253, 253, 253);
        text-align: center;
        padding: 14px 16px;
        text-decoration: none;
    }
 
</style>