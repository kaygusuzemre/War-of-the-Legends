<template>
    <b-container id="heroes" class="container justify-content-center text-center">
        <h2>Heroes</h2>
        <b-row class="my-3 justify-content-start">
            <b-col lg="3" sm="6">
                <b-card class="Card1 bg-dark text-white m-3"
                    img-src="https://images.contentstack.io/v3/assets/blt731acb42bb3d1659/blt570145160dd39dca/5db05fa8347d1c6baa57be25/RiotX_ChampionList_aatrox.jpg?quality=90&width=250 fluid">
                    <b-card-title>My card</b-card-title>
                    <b-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, molestias!
                    </b-card-text>
                    <!-- <template #footer>
                        <span>updated 3 months ago</span>
                    </template> -->
                    <a href="https://www.leagueoflegends.com/de-de/champions/aatrox/" class="stretched-link"></a>
                </b-card>
            </b-col>
            <b-col lg="3" sm="6">
                <b-card class="Card1 bg-dark text-white m-3"
                    img-src="https://images.contentstack.io/v3/assets/blt731acb42bb3d1659/blt9f765d79de67f50e/629ea266a3e9730f695d114a/RiotX_ChampionList_belveth.jpg?quality=90&width=250 fluid">
                    <b-card-title>My card</b-card-title>
                    <b-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, molestias!
                    </b-card-text>
                    <a href="https://www.leagueoflegends.com/de-de/champions/aatrox/" class="stretched-link"></a>
                </b-card>
            </b-col>
            <b-col lg="3" sm="6">
                <b-card class="Card1 bg-dark text-white m-3"
                    img-src="https://images.contentstack.io/v3/assets/blt731acb42bb3d1659/blt4dfb71de3ddc8166/5db05fb13a326d6df6c0e7ad/RiotX_ChampionList_chogath.jpg?quality=90&width=250 fluid">
                    <b-card-title>My card</b-card-title>
                    <b-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, molestias!
                    </b-card-text>
                    <a href="https://www.leagueoflegends.com/de-de/champions/aatrox/" class="stretched-link"></a>
                </b-card>
            </b-col>
            <b-col lg="3" sm="6">
                <b-card class="Card1 bg-dark text-white m-3"
                    img-src="https://images.contentstack.io/v3/assets/blt731acb42bb3d1659/blt1151ac1242311053/61b1ea65aeb5451282be2468/RiotX_ChampionList_fiddlesticks_v2.jpg?quality=90&width=250 fluid">
                    <b-card-title>My card</b-card-title>
                    <b-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, molestias!
                    </b-card-text>
                    <a href="https://www.leagueoflegends.com/de-de/champions/aatrox/" class="stretched-link"></a>
                </b-card>
            </b-col>
            <b-col lg="3" sm="6">
                <b-card class="Card1 bg-dark text-white m-3"
                    img-src="https://images.contentstack.io/v3/assets/blt731acb42bb3d1659/blt5fff73e1df1873de/5db05fce7d28b76cfe4397f5/RiotX_ChampionList_ivern.jpg?quality=90&width=250 fluid">
                    <b-card-title>My card</b-card-title>
                    <b-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, molestias!
                    </b-card-text>
                    <a href="https://www.leagueoflegends.com/de-de/champions/aatrox/" class="stretched-link"></a>
                </b-card>
            </b-col>
            <b-col lg="3" sm="6">
                <b-card class="Card1 bg-dark text-white m-3"
                    img-src="https://images.contentstack.io/v3/assets/blt731acb42bb3d1659/blt69b8fad9d1e78514/5db05fd7df78486c826dcd0c/RiotX_ChampionList_karthus.jpg?quality=90&width=250 fluid">
                    <b-card-title>My card</b-card-title>
                    <b-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, molestias!
                    </b-card-text>
                    <a href="https://www.leagueoflegends.com/de-de/champions/aatrox/" class="stretched-link"></a>
                </b-card>
            </b-col>
            <b-col lg="3" sm="6">
                <b-card class="Card1 bg-dark text-white m-3"
                    img-src="https://images.contentstack.io/v3/assets/blt731acb42bb3d1659/blte24b4c6ec1beebb9/5db05fbddf78486c826dccf4/RiotX_ChampionList_evelynn.jpg?quality=90&width=250 fluid">
                    <b-card-title>My card</b-card-title>
                    <b-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, molestias!
                    </b-card-text>
                    <a href="https://www.leagueoflegends.com/de-de/champions/aatrox/" class="stretched-link"></a>
                </b-card>
            </b-col>
            <b-col lg="3" sm="6">
                <b-card class="Card1 bg-dark text-white m-3"
                    img-src="https://images.contentstack.io/v3/assets/blt731acb42bb3d1659/bltc0f0007660b7a07b/5db05fd689fb926b491ed823/RiotX_ChampionList_kindred.jpg?quality=90&width=250 fluid">
                    <b-card-title>My card</b-card-title>
                    <b-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, molestias!
                    </b-card-text>
                    <a href="https://www.leagueoflegends.com/de-de/champions/aatrox/" class="stretched-link"></a>
                </b-card>
            </b-col>
        </b-row>
    </b-container>
</template>

<script>
export default {
    name: "CardsOne",
    data() {
        return {
            active: ' ',
        }
    },
    methods: {
        setActive(value) {
            this.active = value;
        }
    }
};
</script>

<style lang="scss">
.Card1 {
    transition: all 0.5s ease-in-out;
}

.Card1:hover {
    transform: scale(1.05);
    // transform: skewX(-3deg);
}
</style>