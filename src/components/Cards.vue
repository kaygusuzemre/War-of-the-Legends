<template>

    <b-container class="justify-content-center text-center">
        <h1 class="text-light m-5">Heroes</h1>
        <b-row class="my-3 justify-content-md-center">
            <b-col lg="4" sm="12">
                <b-card class="bg-dark text-white m-3"
                    img-src="https://images.contentstack.io/v3/assets/blt731acb42bb3d1659/blt570145160dd39dca/5db05fa8347d1c6baa57be25/RiotX_ChampionList_aatrox.jpg?quality=90&width=250 fluid">
                    <b-card-title>My card</b-card-title>
                    <b-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, molestias!
                    </b-card-text>
                    <template #footer>
                        <small class="text-muted">Last updated 3 mins ago</small>
                    </template>
                    <a href="https://www.leagueoflegends.com/de-de/champions/aatrox/" class="stretched-link"></a>
                </b-card>
            </b-col>
            <b-col lg="4" sm="12">
                <b-card class="bg-dark text-white m-3"
                    img-src="https://images.contentstack.io/v3/assets/blt731acb42bb3d1659/blt9f765d79de67f50e/629ea266a3e9730f695d114a/RiotX_ChampionList_belveth.jpg?quality=90&width=250 fluid">
                    <b-card-title>My card</b-card-title>
                    <b-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, molestias!
                    </b-card-text>
                    <template #footer>
                        <small class="text-muted">Last updated 3 mins ago</small>
                    </template>
                    <a href="https://www.leagueoflegends.com/de-de/champions/aatrox/" class="stretched-link"></a>
                </b-card>
            </b-col>
            <b-col lg="4" sm="12">
                <b-card class="bg-dark text-white m-3"
                    img-src="https://images.contentstack.io/v3/assets/blt731acb42bb3d1659/blt4dfb71de3ddc8166/5db05fb13a326d6df6c0e7ad/RiotX_ChampionList_chogath.jpg?quality=90&width=250 fluid">
                    <b-card-title>My card</b-card-title>
                    <b-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, molestias!
                    </b-card-text>
                    <template #footer>
                        <small class="text-muted">Last updated 3 mins ago</small>
                    </template>
                    <a href="https://www.leagueoflegends.com/de-de/champions/aatrox/" class="stretched-link"></a>
                </b-card>
            </b-col>
        </b-row>

        <hr>

        <b-row class="my-3">
            <b-col lg="4" sm="12">
                <b-card class="bg-dark text-white m-3"
                    img-src="https://images.contentstack.io/v3/assets/blt731acb42bb3d1659/blt1151ac1242311053/61b1ea65aeb5451282be2468/RiotX_ChampionList_fiddlesticks_v2.jpg?quality=90&width=250 fluid">
                    <b-card-title>My card</b-card-title>
                    <b-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, molestias!
                    </b-card-text>
                    <template #footer>
                        <small class="text-muted">Last updated 3 mins ago</small>
                    </template>
                    <a href="https://www.leagueoflegends.com/de-de/champions/aatrox/" class="stretched-link"></a>
                </b-card>
            </b-col>
            <b-col lg="4" sm="12">
                <b-card class="bg-dark text-white m-3"
                    img-src="https://images.contentstack.io/v3/assets/blt731acb42bb3d1659/blt5fff73e1df1873de/5db05fce7d28b76cfe4397f5/RiotX_ChampionList_ivern.jpg?quality=90&width=250 fluid">
                    <b-card-title>My card</b-card-title>
                    <b-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, molestias!
                    </b-card-text>
                    <template #footer>
                        <small class="text-muted">Last updated 3 mins ago</small>
                    </template>
                    <a href="https://www.leagueoflegends.com/de-de/champions/aatrox/" class="stretched-link"></a>
                </b-card>
            </b-col>
            <b-col id="col6" v-b-hover="handleHover" lg="4" sm="12">
                <transition>
                    <b-card v-if="isHovered" class="bg-danger text-white m-3"
                        img-src="https://images.contentstack.io/v3/assets/blt731acb42bb3d1659/blt69b8fad9d1e78514/5db05fd7df78486c826dcd0c/RiotX_ChampionList_karthus.jpg?quality=90&width=250 fluid">
                        <b-card-title>My card</b-card-title>
                        <b-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, molestias!
                        </b-card-text>
                        <template #footer>
                            <small class="text-muted">Last updated 3 mins ago</small>
                        </template>
                        <a href="https://www.leagueoflegends.com/de-de/champions/aatrox/" class="stretched-link"></a>
                    </b-card>

                    <b-card v-else class="bg-dark text-white m-3"
                        img-src="https://images.contentstack.io/v3/assets/blt731acb42bb3d1659/blt69b8fad9d1e78514/5db05fd7df78486c826dcd0c/RiotX_ChampionList_karthus.jpg?quality=90&width=250 fluid">
                        <b-card-title>My card</b-card-title>
                        <b-card-text>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, molestias!
                        </b-card-text>
                        <template #footer>
                            <small class="text-muted">Last updated 3 mins ago</small>
                        </template>
                        <a href="https://www.leagueoflegends.com/de-de/champions/aatrox/" class="stretched-link"></a>
                    </b-card>
                </transition>
            </b-col>
        </b-row>
    </b-container>
</template>

<script>
export default {
    name: "CardsOne",
    data() {
        return {
            isHovered: false
        }
    },
    methods: {
        handleHover(hovered) {
            this.isHovered = hovered
        }
    }
};
</script>

<style>
.visible {
    visibility: visible;
}

.invisible {
    visibility: hidden;
}

.view-enter-active {
    transition: opacity 0.5s ease-in-out;
}

.view-leave-active {
    transition: transform 0.5s ease;
}
</style>
