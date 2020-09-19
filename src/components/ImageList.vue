<template>
    <v-container>
        <v-row>
      <v-col v-bind:key="item.id" v-for="item in items.hits" sm="4" cols="12">
                <v-card>
                    <v-card-title>
                                                
                    </v-card-title>

                </v-card>
            </v-col>
        </v-row>
    </v-container>

    
</template>

<script>
export default {
    name:'ImageList',
    props:[
        "items"
    ]
}
</script>