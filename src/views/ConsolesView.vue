<template lang="">
    <div>
    Consoles Page
    </div>
    <div>
        <slot v-for = "console in gaming_consoles" :key="console">

            <card-comp>
                {{console.name}}
                {{console.storage}}
                {{console.manufacturer}}
                {{console.release_year}}
                {{console.best_selling_game}}
                {{console.price}}
            </card-comp>
        </slot>
        
    </div>
</template>
<script>
import CardComp from '@/components/CardComp.vue'
export default {
    data(){
        return{
            "gaming_consoles":[
        {
            "name": "PlayStation 5",
            "manufacturer": "Sony",
            "release_year": 2020,
            "storage": "825GB SSD",
            "price": 499,
            "best_selling_game": "Spider-Man: Miles Morales"
        },
        {
            "name": "Xbox Series X",
            "manufacturer": "Microsoft",
            "release_year": 2020,
            "storage": "1TB SSD",
            "price": 499,
            "best_selling_game": "Halo Infinite"
        },
        {
            "name": "Nintendo Switch",
            "manufacturer": "Nintendo",
            "release_year": 2017,
            "storage": "32GB",
            "price": 299,
            "best_selling_game": "Mario Kart 8 Deluxe"
        },
        {
            "name": "Steam Deck",
            "manufacturer": "Valve",
            "release_year": 2022,
            "storage": "64GB eMMC",
            "price": 399,
            "best_selling_game": "Elden Ring"
        },
        {
            "name": "PlayStation 4 Pro",
            "manufacturer": "Sony",
            "release_year": 2016,
            "storage": "1TB HDD",
            "price": 399,
            "best_selling_game": "God of War (2018)"
        }
    ]
        }
    },
    components:{
        CardComp
    }
     
}
</script>
<style lang="">
    
</style>